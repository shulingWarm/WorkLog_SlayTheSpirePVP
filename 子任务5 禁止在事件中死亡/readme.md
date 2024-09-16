# 背景
- 为了适应两个的多人2v2环境，需要禁止玩家在地图的随机事件中死亡
- 采取的手段是当事件涉及到掉血时，把掉血量的上限修改为当前HP-1
- 由于每个事件的掉血逻辑都是单独实现的，因此需要对这些选项做分类讨论。

# 工作流程
- [DONE] 重新实现全知头骨
	- 背景: 全知头骨事件是最容易在事件中死亡的事件，因此需要先对这个事件做特殊处理。
	- 结果: 目前每次更新全知头骨的受伤数时，先判断角色目前的血量是否可以承受这个伤害。
- [DONE] 重新实现打防之光
	- 结果: 如果生命值不够14的时候，禁止选择升级牌的选项。
- [DONE] 临时bug解决: 解决壁垒结算相关的bug.
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/7c89e0ad105a96a09b865c68137d9973520f8bdb
- [DONE] 临时bug解决: 解决使用腾跃后玩家回合卡死的bug
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/639107f281e7e3a667abf6e46ce46bcd8554287d
- [DONE] 临时bug解决: 解决Steam联机时无法使用滚轮的bug
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/b2edb557eaa7619d94e40a2d21ef9759cbd89b52
- [DONE] 临时bug解决: 添加2v2模式下的斩杀同步，这样可以给各种血量不同步的问题兜底
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/f9f87e629c122a845882de6cca90d7ac0877f7f3
- [DONE] 回合内反伤死亡造成的bug
	- 背景: 如果玩家回合内被荆棘反伤死亡，下家玩家无法正常开始回合，需要解决这个bug.
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/6f194da211ac88fe0bf79802fbeea92cea0e5c7c
- [TO-DO] 重新实现死灵之书事件 
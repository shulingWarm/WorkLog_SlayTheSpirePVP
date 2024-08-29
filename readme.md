# 目标
- 令杀戮尖塔pvpmod成为一个游戏体验良好，平衡良好且具有游戏深度的mod

# 工作过程记录
- [DONE] 子任务1 添加三国杀2v2形式的座次顺序
- [DONE] BUG处理: 有时会提前摸下回合的牌
    - 结果: 修改后连续测试20回合未再出现bug.
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/commit/9e8e30b99c6317cbb524dde900423657dbf4471d
- [DONE] BUG处理: 解决第二场战斗出牌顺序错误的问题
    - 背景: 在第二场战斗开始时，双方都无法出牌。
    - 结果: 解决后，第二场战斗的出牌顺序符合游戏设定。
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/commit/adf637df151caab0a2084ab0a69a436d6b7ecd9d
- [DONE] BUG处理: 第二场战斗4号位会先摸牌再弃牌
    - 背景: 第二场战斗的先手方是1,4号位，但4号位会先摸牌再立刻结束回合
    - 结果: 解决后，第二场战斗的4号位在战斗开始时不会先摸牌再弃牌。
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/commit/e8ec183af3ef271a98a593756fb8efab0bee5f77
- [DONE] BUG处理: 第二场战斗变为1,3对战2,4,本来应该是14对应23的
- [TO-DO] 添加回游戏中的老头表(时间扭曲)
    - 背景: 由于2v2配置的出牌需要分别结算，老头表的buff需要重新实现。
- [TO-DO] 在游戏配置页面添加禁卡功能
- [TO-DO] 给游戏中每个角色添加一批给目标上脆弱的牌
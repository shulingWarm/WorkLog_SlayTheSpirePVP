# 目标
- 由于与外国友人建立了bug反馈的通道:https://docs.google.com/document/d/1RievMcF37ZdpeJp78kLPvbqcsF6ISPTNxdsDbnwNJVg/edit?tab=t.0 ，后续可能会频繁涉及到功能与bug修改并行的情况，所以开辟了一个子任务专门用于处理各种BUG

# 工作过程
- [DONE] 解决猎人死后她施加的毒变得无效的bug.
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/893568d1f7507e0db63aeb8d20834d93a00fd558
- [DONE] 解决失败的一方先死的无法结束战斗。
	- 背景: 这是一个可以稳定复现的bug,2v2的情况下，败方先死的一个无法结束战斗，会卡在那里。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/ce8cbe8af40afc6131223ba46b45ba3f58ed0d57
- [DONE] 在聊天框里面添加玩家所在楼层的状态信息，用于debug。
	- 背景: 由于玩家反馈所有玩家进入房间后无法开始战斗，添加这一条信息用于收集玩家的状态。
- [DONE] 修改一些遗物的英文描述。
	- Stage:
		- [DONE] 由于燃烧之血的词条描述是用patch更改的，因此需要将它重新修改成语言包的形式。
		- [DONE] 修改其他遗物的英文描述。
- [DONE] 添加一个config选项用于指定是否允许使用控制台。
	- Stage:
		- [DONE] 添加了用于实现ConsoleOption的选项。
		- [DONE] 测试添加控制台的选项。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/62bc2b5f319ec523a747ccabfef5e7ae230c8dbe
- [GIVE-UP] 解决1v1被毒死时无法正常结束游戏的bug.
	- [DOING] 试图复现被毒死时无法结束回合的bug，但没有复现出来。
	- 放弃原因: 目前无法复现这个bug.
- [DONE] 合并测试新的pom.xml管理方案。
	- 背景: Luc重写了pom.xml,现在pom.xml更规范了。
	- 结果: 测试之后，使用新的pom.xml仍然可以正常构建工程。
- [GIVE-UP] 测试坚不可摧打满的情况下使用审判击杀会卡死。
	- 放弃原因: 没能复现出这个bug.
- [DONE] 移除正常的添水和狗圈。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/4a02fa676d0ab65bee6a40e1ba9954dce4a06ea5
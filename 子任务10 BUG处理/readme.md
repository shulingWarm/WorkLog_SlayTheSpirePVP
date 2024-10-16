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
- [TO-DO] 修改一些卡牌的英文描述。
- [TO-DO] 添加一个config选项用于指定是否允许使用控制台。
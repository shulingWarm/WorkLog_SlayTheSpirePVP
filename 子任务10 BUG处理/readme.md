# 目标
- 由于与外国友人建立了bug反馈的通道:https://docs.google.com/document/d/1RievMcF37ZdpeJp78kLPvbqcsF6ISPTNxdsDbnwNJVg/edit?tab=t.0 ，后续可能会频繁涉及到功能与bug修改并行的情况，所以开辟了一个子任务专门用于处理各种BUG

# 工作过程
- [DONE] 解决猎人死后她施加的毒变得无效的bug.
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/893568d1f7507e0db63aeb8d20834d93a00fd558
- [DOING] 解决失败的一方先死的无法结束战斗。
	- 背景: 这是一个可以稳定复现的bug,2v2的情况下，败方先死的一个无法结束战斗，会卡在那里。
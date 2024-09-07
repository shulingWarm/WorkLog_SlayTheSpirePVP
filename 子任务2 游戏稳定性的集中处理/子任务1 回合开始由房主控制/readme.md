# 背景
- 将玩家回合开始的逻辑改成由房主来控制
- 以前是每个玩家本地都维护一份回合状态，这样一旦回合状态不同步就会出现bug

# 工作过程
- [DONE] 添加定义SeatManager,用于管理一个座位中的玩家的信息
	- 动机: 做这个东西是因为一个座位上可能有多个玩家，为了兼容另外一种同一队的玩家可以同时出牌的模式
- [DONE] 将TurnManager中更换轮次换成由SeatManager来处理
- [DONE] 在SeatManager中实现发送轮次启动的信息，添加一个相应的通信Event
- [DONE] 当前座位的玩家都出牌结束时，通知下一个座位的玩家开始出牌。
- [DONE] 测试中发现一个bug, 2v2中有玩家死亡时，无法正常跳过它的回合。
	- PR: https://github.com/shulingWarm/PVP-in-the-spire/commit/06b0f11b96732a1cf6d84b3e678325808974fdcd
- [DONE] 在虚拟机里面用真实的服务器来测试。
	- 结果: 用真实的steam服务器网络测试也都是正常的。

# 结果
- 可以用真实steam联机的情况下正常完成一局游戏并且没有出现bug
 
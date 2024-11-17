# 目标
- 添加禁卡功能，方便玩家自定义卡池。

# 工作过程
- [DONE] 试用目前其他人已经实现好的卡牌过滤器功能，然后提出适合pvpmod的卡牌过滤器的方案。
	- 结果: 参考了CardFilterMod,卡牌过滤功能的页面类似于百科大全的页面，显示所有的卡牌然后让玩家设置
- [DOING] 实现可自由修改的浏览卡牌页面，后面会基于这个页面做禁牌功能。
	- 状态:
		- [DONE] 找到了用于显示卡牌库的类。
		- [DONE] 将卡牌库放到一个PVP的标准AbstractPage里面。
		- [DONE] 在测试页面添加AbstractPage测试时，open的时候遇到了空指针错误。
			- CardLibraryScreen里面有basemod的patch,因此需要先把它独立出来。
		- [DONE] 将原版游戏中的CardLibraryScreen解耦出来变成一个完全独立的类。
		- [DOING] 由于游戏里面上下文关系，构造CardLibrary的时候需要在特定的位置，所以需要和原版的游戏保持一致。
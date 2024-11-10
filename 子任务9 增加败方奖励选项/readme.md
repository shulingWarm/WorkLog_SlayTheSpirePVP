# 目标
- 增加败方的奖励选项，包括增加金卡三选一，获得金币之类的。

# 工作过程
- [DONE] 添加死亡后获得金币的功能。
	- 背景: 这一步不需要添加控制打开的逻辑，只需要确保这个功能可以正常实现就行。
	- 状态:
		- [DONE] 测试发现，在玩家逃跑时把currRoom里面的smoke选项设置成false就可以正常获得所有奖励。
		- [DONE] 在不把smoke设置成true的情况下，跳过setupItemReward即可跳过获得奖励的过程。
		- [DONE] 测试在setupItemReward里面能不能添加自定义的奖励项目。
	- 结果: 可以直接覆盖setupItemReward来指定败方的奖励。
- [DONE] 在config页面添加败方获得金币的功能。
	- 结果: 添加了在界面里面设置的金币奖励选项。
- [DONE] 添加败方获得金卡的功能。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/f0da1253dec541a1f6422cfd36e5145bd301b40b

# 结果:
- 目前已经可以正常在用户界面设置败者奖励选项，并且在战斗后也可以正常生效。
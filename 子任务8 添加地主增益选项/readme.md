# 目标
- 添加若干地主增益选项，包括总是先手，没有先手处罚。开局固定多一费，血量翻倍之类的。

# 工作记录
- [DONE] 子任务1 实现多选项option的UI
- [DONE] 添加地主总是先手的选项。
	- [DONE] 在config界面添加总是先手的选项。
	- [DONE] 实现一种总是先手的座次管理器。
	- [DONE] 在新建座次管理器的时候，如果打开了地主总是先手的选项，就启用地主先手的座次管理器。
	- [DONE] 当点击config页面里面的选项时，调用通信更新其他玩家的页面。
	- [DONE] 测试更新Toggle选项时，在其他玩家的界面中也会同步更新。
	- [DONE] 测试地主总是先手的效果
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/337ef4e91af7293be764dd9d60e6e5b809d79487
- [DONE] 添加地主没有先手处罚的选项
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/61b5fe8cfacb48389d8dda0376c522571a3d88ef
- [DONE] 地主开局固定多一费。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/9cd55a3b15ca61446d92e6eae093dd386820c26c
- [DONE] 地主多获得一条尾巴
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/5bb999ed61a31a7b4432018709ee2059e12915bf
- [DONE] 录视频说明目前的地主增益选项
	- 结果: https://www.bilibili.com/video/BV1rV23YdENg
- [TO-DO] 修改ToggleOption的点击范围
	- 背景: 目前的ToggleOption的点击范围是向右扩展的，为了与实际的使用保持一致，这里改成向左扩展。

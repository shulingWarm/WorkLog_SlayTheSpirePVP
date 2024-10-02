# 目标
- 由于以前制作的界面都只有单个选项，但这次的地主增益是多选项配置
- 之前并没有相关的UI逻辑，因此需要单独实现这个UI素材

# 工作记录
- [DONE] 研究怎样在界面中添加用于多选的ToggleButton
	- 结论: 关键就是它怎样使用它原生自带的ToggleButton
- [DONE] 在游戏里面测试单独使用ToggleButton的效果
	- 目的: 这是为了指导后面使用ToggleButton的效果，方便决定后续的修改方向。
	- 结果: 添加ToggleButton会出现一个新的Toggle按钮。
- [DOING] 制作由用户设置响应事件的ToggleButton
	- 目的: 
		- 原生的ToggleButton只能在新建的时候就指定对应的功能
		- 现在需要设置一个专门的Interface,然后由Interface去处理点击回调。
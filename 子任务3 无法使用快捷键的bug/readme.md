# 背景
- 通过steam联机时，房主在进入游戏后无法使用快捷键。
- 非房主或者非steam联机的情况下可以使用快捷键。
- 打开聊天窗口再关闭后可以使用快捷键。

# 工作记录
- [DONE] 在游戏源码中查找响应快捷键的逻辑，哪些条件下快捷键会无法使用。
	- 游戏中检查是否按下快捷键的位置在这里： InputAction.isJustPressed
- [DONE] 在进入游戏时关闭对快捷键的禁用。
	- 背景: 最后发现这是pvpmod自身造成的bug,当创建房间时会涉及到文本输入框，而文本输入框会禁用快捷键。在进入游戏之后需要解除这种禁用。
	- Commit: https://github.com/shulingWarm/PVP-in-the-spire/commit/3608135dba197044ae689d064d4ee136f6e0def0

# 结果
- 目前任何情况下都可能正常使用快捷键，不会再出现无法使用快捷键的情况。
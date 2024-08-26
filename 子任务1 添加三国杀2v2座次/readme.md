# 背景
- 目前2v2的模式的座位轮流模式是两个队伍之间轮流出牌
- 需要改成类似于三国杀那个1,2,3,4号位那种形式，1,4号位一队, 2,3号位一队

# 目标
- 最终会在2v2模式里面添加一个自定义选项，允许玩家选择队伍之间轮流出牌或者1,2,3,4号位轮流

# 工作流程
- [DONE] 将目前的队伍间轮流的模式模块化，变成独立的接口
    - 结果: 该模块被设置为 TurnManager
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/blob/master/src/main/java/WarlordEmblem/PlayerManagement/TurnManager.java
- [DONE] 制作三国杀式的2v2轮次方式。
    - 代码参考: https://github.com/shulingWarm/PVP-in-the-spire/blob/master/src/main/java/WarlordEmblem/PlayerManagement/PersonTurnManager.java
- [DONE] 添加config界面的选项，允许玩家自定义2v2式的方式或者和队友同时出牌。
    - 代码参考: https://github.com/shulingWarm/PVP-in-the-spire/blob/master/src/main/java/UI/configOptions/TurnStrategyOption.java

# 结果
- 目前已经支持自定义为三国杀2v2形式的坐次顺序
- 演示视频: https://www.bilibili.com/video/BV1KtsJeXEhA
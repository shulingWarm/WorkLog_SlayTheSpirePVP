# 背景
与真人玩家测试用steam远程联机，集中出现了若干bug
- 在玩家准备房间里面配置时，当有玩家准备时出现闪退
- 有时战斗开始时的敌人的血量为零，明显是玩家的血量信息没有正常初始化
- 所有玩家准备后，有的玩家无法正常进入游戏。

# 工作过程
- [DONE] 添加玩家准备信息处理的空指针检查
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/commit/818b76dec320f8527375af637b778fa9d2bfa56c
- [DONE] 解决战斗开始时血量为零的bug
    - 参考: https://github.com/shulingWarm/PVP-in-the-spire/commit/ec640ccfe30759ee0be4b27294f8e7a1f1af8b87
- [DONE] 子任务1 改成回合开始条件完全由房主控制
    - 动机: 由于目前的pvp总是出现双方玩家回合都无法开始的情况，改成回合开始条件完全由房主控制可以增加回合开始的稳定性。
    
# 结果
- 目前关于回合控制的内容已经稳定，可以用steam联机稳定进行一局游戏。
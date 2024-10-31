# 8月
- [DONE] 添加2v2中类似于三国杀的座次顺序
    - 效果演示: https://www.bilibili.com/video/BV1KtsJeXEhA
- [DONE] BUG处理: 有时会提前摸下回合的牌
    - PR: https://github.com/shulingWarm/PVP-in-the-spire/commit/adf637df151caab0a2084ab0a69a436d6b7ecd9d
- [DOING] 解决steam远程联机时影响游戏稳定性的bug

# 9月
- [DONE] 解决Steam远程联机时的稳定性问题，目前不会再Steam联机时回合卡死。
- [DONE] 聊天界面优化: 允许使用快捷键打开和关闭聊天框，聊天信息会显示发送者。
- [DONE] 禁止玩家死在事件中，重新实现了[全知头骨]，[诅咒之书]等事件。
- [DONE] 在游戏中添加了[时间扭曲]。
    - 演示视频: https://www.bilibili.com/video/BV1Lzxge7EfG
- [DONE] 部分BOSS遗物效果的修改，重新实现了狗圈、添水和绿帽。
- [DOING] 添加地主增益选项。

# 10月
- [DONE] 添加地主增益选项
    - 演示视频: https://www.bilibili.com/video/BV1rV23YdENg
- [DOING] BUG集中修复
    - 背景: 由于Ruben和Luc总结了bug记录的文档，因此需要集中处理这些bug.
    - [DONE] 猎人死亡后毒不触发。
    - [DONE] 解决2v2时，失败队伍中先死的玩家无法正常结束战斗，会被卡住。
    - [DONE] 移除了游戏中普通的绿帽和狗圈。
    - [DONE] 修复[灵体外质]的bug,确保只有Normal类型的伤害才会被偷钱
    - [DONE] 修复[百年积木]的bug,有时第二场战斗它不触发。
    - [DONE] 当有玩家在游戏中退出时，弹出结束游戏的按钮。
    - [DOING] Steam远程联机时，地主增益选项无法同步给新进入房间的玩家。
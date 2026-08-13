# 运行时模型入口

优化后的正式 GLB 位于 `public/models/jinsha/`。游戏会按稳定资产 ID 自动加载；
仍可在游戏中按 `F2` 打开编辑器，为选中容器加载其他本地 GLB 做临时对比。

约定的正式文件名：

- `bronze-giant.glb`：青铜立人巨物版，已接入。
- `ruin-gate.glb`：原文件误命名为 iron gate，实际为青铜神树，已接入两处。
- `mask-a.glb` / `mask-b.glb`：头像面具与纵目面具，已接入。
- `ancient-bird.glb`：青铜神鸟守望者，已接入。
- `golden-wand.glb`：金杖遗物，已接入。
- `sun-wheel.glb`：青铜轮形器遗物，仅作场景点缀，不代替太阳神鸟。
- `sunbird-emblem.glb`：正式太阳神鸟金饰模型；运行时保留基础色纹理，并覆盖为高金属度、低粗糙度的暗金材质。
- 鱼群继续使用程序化实例资产。
- `player/alice-xbot.glb`：来自 Alice 项目的 Mixamo 人形主角，作为巨物尺度参照。

正式接入时应从文件 URL 加载，不应依赖浏览器本地文件。原始高模继续保存在
`model/` 并排除出 Git，本目录只放网页优化后产物。

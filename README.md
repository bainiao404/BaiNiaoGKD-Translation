# BaiNiaoGKD Translation（BNT 翻译产物）

本仓库由白鸟 GKD 翻译工具自动发布，请勿手工编辑。

## 结构

- `index.json` —— 总索引（structureVersion = 2，languages → games → 包元信息）
- `<语言>/<游戏>/manifest.json + speaker.txt + chunks/*.txt` —— BNT 1.1 翻译包（规范见主仓库 specs/BNT_TRANSLATION_SPEC.md）
- `zips/<语言>-<游戏>.zip` —— 每游戏全量包（启动器整目录同步用）

## 消费

启动器「更多 → 翻译更新」按 index.json 检查并同步；游戏运行时按场景懒加载 `chunks/` 并动态回源缺失文本。

最近发布：2026-10-30T00:17:35.845Z

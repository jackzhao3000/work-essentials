# 来源

- 请求地址：https://github.com/hugohe3/ppt-master
- 规范仓库：https://github.com/hugohe3/ppt-master （2026-10-19 核对，仓库存在；技能元数据中的 `official_repository` 同此地址）
- 默认分支：`main`
- 快照提交：`c350bc31e6d43b7bcf5234183d650ba8f9f4c9d7`
- 上游提交时间：2026-10-19
- 镜像日期：2026-10-19
- 技能版本：6.7.2（见 `skills/ppt-master/SKILL.md` 元数据）
- 许可证：MIT。版权声明为 Copyright (c) 2025-2026 Hugo He。许可文本见本目录 `LICENSE` 与 `skills/ppt-master/LICENSE`。本镜像不改变该许可证。

## 收录

技能文档与导出脚本，约 6 MB：

- 仓库说明：`README.md`、`README_CN.md`、`LICENSE`、`requirements.txt`
- 技能入口与署名页：`skills/ppt-master/SKILL.md`、`LICENSE`、`requirements.txt`、`SPONSORS.md`、`SPONSORS_CN.md`
- 工作流：`skills/ppt-master/workflows/`
- 参考说明：`skills/ppt-master/references/`（对照图 webp 已去掉，保留文字与小型 json 索引）
- 导出脚本与说明：
  - `scripts/svg_to_pptx.py` 与 `scripts/svg_to_pptx/`
  - `scripts/pptx_to_svg.py` 与 `scripts/pptx_to_svg/`
  - `scripts/source_to_md.py` 与 `scripts/source_to_md/`
  - `scripts/README.md`、`scripts/docs/`、`scripts/attribution_guard.py`
- 轻量模板（Markdown / SVG / 小型 json）：`templates/styles/`、`templates/layouts/`、`templates/charts/`、`templates/tables/`、`templates/schemas/`，以及模板目录下的写作说明

## 未收录

这些路径留在上游，避免把缓存和素材包搬进个人库：

- `templates/icons/`（约 1.2 万个图标 SVG）及其第三方声明
- `templates/sounds/`（WAV 音效库）
- `templates/brands/`、`templates/decks/` 里的品牌与成套模板素材
- `references/ai-image-comparison/` 下的 webp 对照图
- `docs/assets` 中的预览大图、gif 与赞助商标
- 测试夹具、确认界面静态资源、`.env.example`
- 完整性门禁依赖的其余同级脚本（例如 `scripts/console_encoding.py`）

`scripts/svg_to_pptx.py` 在运行前会调用 `attribution_guard.py`。该检查要求官方完整分发包。精选副本按上游的设计不会通过这道门，完整安装请使用规范仓库。

仓库根目录的 README 仍是上游原文，其中指向 `docs/` 与赞助商图片的相对链接在本镜像里没有对应文件。

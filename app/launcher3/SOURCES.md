[首页](../../README.md) / [Launcher3](README.md) / 来源记录

# 来源与整理记录

首批文档于 **2026-11-20** 从本人飞书知识库读取，保留完整技术正文、图表和各篇源码基线。以下 revision 是导出接口返回的文档版本，不是 Git commit。

## 原文与版本

| 文档 | 飞书原文 | revision | 原文分析日期 | 图表 |
| :--- | :--- | :---: | :---: | :---: |
| [Launcher3 View层级与状态机架构详解](view-and-state.md) | [原文](https://cvte.feishu.cn/wiki/THR8w93Zii4U9UkaodUcWzfMnKg) | 25 | 2026-10-19 | 24 |
| [OSLauncher3 Workspace 数据库设计：模型、演进与精妙之处](workspace-database.md) | [原文](https://cvte.feishu.cn/wiki/A81hwfpBwifc8CkK5S3cvb8tnUc) | 17 | 2026-10-19 | 7 |
| [OSLauncher3 图标加载架构与动态图标设计](icon-loading.md) | [原文](https://cvte.feishu.cn/wiki/WzitwmPx3iPZGTkQ82Yc9L62nwb) | 5 | 2026-11-20 | 12 |
| [OSLauncher3 与 SystemUI 协作详解：Binder、手势、转场与窗口管理](systemui-integration.md) | [原文](https://cvte.feishu.cn/wiki/CPgbwBlMiik7Gok3zbvcKHdRnUr) | 19 | 2026-10-19 | 5 |
| [OSLauncher3 Overview 实现全景：任务、缩略图、手势与系统动画](overview.md) | [原文](https://cvte.feishu.cn/wiki/BVgRwi5WYiOuFYkbftschMpCntd) | 10 | 2026-11-20 | 14 |

## Launcher 源码基线

| 文档 | 分支 | 完整 commit |
| :--- | :--- | :--- |
| [Launcher3 View层级与状态机架构详解](view-and-state.md) | `em-stable-15` | `5af275b915993e0bfa3c414f7bc4ff51281b1614` |
| [OSLauncher3 Workspace 数据库设计：模型、演进与精妙之处](workspace-database.md) | `em-stable-16` | `7dddb9d7d38d7ec3ee6cb5be261a8510190d9182` |
| [OSLauncher3 图标加载架构与动态图标设计](icon-loading.md) | `em-stable` | `ae97ee43360d19569eb056613f9ec97060343984` |
| [OSLauncher3 与 SystemUI 协作详解：Binder、手势、转场与窗口管理](systemui-integration.md) | `em-stable-16` | `7dddb9d7d38d7ec3ee6cb5be261a8510190d9182` |
| [OSLauncher3 Overview 实现全景：任务、缩略图、手势与系统动画](overview.md) | `em-stable` | `ae97ee43360d19569eb056613f9ec97060343984` |

SystemUI、framework、接口 jar 等额外基线按文章中的原始说明保留。本文档整理没有重新 fetch 分析所涉及的源码仓库，原文中“当前”“默认”等描述仍对应原文的分支、commit 和分析日期。

## 本次整理范围

- 选取知识库中的 5 篇完整技术文章；同名旧稿、需求文档、主题切换问题单及月报未纳入本专题。
- 将飞书标题和 callout 转换为 GitHub Markdown 标题及提示块；保留正文内容与章节关系。
- 增加专题首页、推荐阅读顺序、问题索引、可折叠目录及上一篇／下一篇导航。
- 将本专题内的文章互引改为相对链接；保留飞书原文入口和原有源码索引。
- 修复 SystemUI 协作文章中 9 个 Gitiles 源码 URL 的空格分隔符为标准 `/+/` 分隔符；不更改其 commit 和文件路径。
- 逐张完成 62 张 Mermaid 图的语法与渲染检查，原图均通过，保留原有图表内容。
- 5 篇原文共 62 个 Mermaid 代码块；没有需要迁移的独立图片或嵌入表格附件。

飞书原文与内部源码链接保留原有访问权限。GitHub 正文、表格和图表可以独立阅读。

<details>
<summary>原始 Markdown 的 SHA-256（整理前）</summary>

用于标识本次读取的原文快照；接口响应和本地导出缓存不提交到仓库。

- `view-and-state`：`db0dfae59266992b7dd44de00ce0bab2ede6d7bb46dd75f8b6a6e88b138aa604`
- `workspace-database`：`08fdb20c82d500e8a001427ace252676bd25a505c267ddeeca3ac8ab41d09a85`
- `icon-loading`：`78f7e634bc5a543a6d735f51de041262fca048c5a3c8299b3043d1586298194c`
- `systemui-integration`：`393ff6bb5f716aa8cae734897cab4f1a995d435989be523c27b39fc52f60c22a`
- `overview`：`5698d11aafe002778d059bfe32baef0891c446e65f99c3712a5f4ea1d48d8898`

</details>

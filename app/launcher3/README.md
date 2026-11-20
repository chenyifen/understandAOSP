[首页](../../README.md) / [应用设计](../README.md) / Launcher3

# Launcher3 · 从桌面到系统交互

**一棵 View 树，一份布局模型，一套连接系统窗口的交互协议。**

这个专题把 Launcher3 按界面、数据、图标与系统协作逐层展开。5 篇文章保留原文的技术分析和源码边界，62 张 Mermaid 图可直接在 GitHub 阅读。

## 推荐阅读顺序

| 顺序 | 文档 | 关注点 | 图表 |
| :---: | :--- | :--- | :---: |
| **01** | [View 层级与状态机架构详解](view-and-state.md) | View 树、Z 轴、触摸仲裁、LauncherState 与 StateManager | 24 |
| **02** | [Workspace 数据库设计：模型、演进与精妙之处](workspace-database.md) | favorites、BgDataModel、布局迁移、恢复与多库路由 | 7 |
| **03** | [图标加载架构与动态图标设计](icon-loading.md) | 多级缓存、图标规范化、日历与时钟、进度与徽标 | 12 |
| **04** | [与 SystemUI 协作：Binder、手势、转场与窗口管理](systemui-integration.md) | 双向 Binder、Taskbar、WM Shell、分屏与多显示器 | 5 |
| **05** | [Overview 实现全景：任务、缩略图、手势与系统动画](overview.md) | RecentsAnimation、TaskSnapshot、Live Tile 与 Surface 同步 | 14 |

## 按问题查阅

| 我想弄清楚…… | 建议从哪里开始 |
| :--- | :--- |
| 某个 View 为什么看不见、盖住其他元素或接不到触摸？ | [View 层级与状态机](view-and-state.md) |
| 切到抽屉、Overview 时，原来的桌面去了哪里？ | [View 层级与状态机](view-and-state.md) |
| 图标位置为什么会在恢复、迁移或账号切换后改变？ | [Workspace 数据库](workspace-database.md) |
| 图标为什么显示旧缓存，动态图标如何正确失效？ | [图标加载](icon-loading.md) |
| Launcher、SystemUI、WM Shell 各自负责什么？ | [SystemUI 协作](systemui-integration.md) |
| Taskbar 为什么不属于 Launcher Activity 的 View 树？ | [SystemUI 协作](systemui-integration.md) |
| 最近任务显示的是截图还是真实应用窗口？ | [Overview](overview.md) |
| 手势结束、动画完成与 Surface 释放如何避免黑帧？ | [Overview](overview.md) |

## 源码基线

| 文章 | 原文分析基线 |
| :--- | :--- |
| View 与状态机 | `em-stable-15` · `5af275b91599` |
| Workspace 数据库、SystemUI 协作 | `em-stable-16` · `7dddb9d7d38d` |
| 图标加载、Overview | `em-stable` · `ae97ee43360d` |

这些文章分析的是不同分支和时间点，接口名、配置默认值和定制能力可能不同。跨篇比较时应先对齐基线；本文档整理没有新增源码核验或实机验收结论。

[查看飞书来源、版本与整理记录 →](SOURCES.md)

---

[开始第一篇：View 层级与状态机 →](view-and-state.md)

# EastMG

**二游日历作者。** 把「二次元手游的卡池 / 活动排期」做成一整套跨端工具——浏览器扩展、PWA、Windows 任务栏小组件、DeepSeek Harness 插件——四端共用同一份抓取核心。

数据只从各游戏**官方公告与社区 Wiki** 抓取，保留来源与抓取时间，不经过任何中转服务器。

[![Edge Add-ons](https://img.shields.io/badge/Edge%20Add--ons-%E5%B7%B2%E4%B8%8A%E6%9E%B6-0C59A4)](https://microsoftedge.microsoft.com/addons/detail/mkfokebcmknjnbjceabimdchdfhbdhhc)
[![npm core](https://img.shields.io/npm/v/gacha-calendar-core?label=gacha-calendar-core)](https://www.npmjs.com/package/gacha-calendar-core)
[![npm plugin](https://img.shields.io/npm/v/dsh-gacha-calendar?label=dsh-gacha-calendar)](https://www.npmjs.com/package/dsh-gacha-calendar)

---

## 🗓 二游日历（Gacha Calendar）

> 28 款二次元手游的当期卡池与活动起止，一处解析、四处呈现。

| 端 | 形态 | 入口 | 状态 |
|---|---|---|---|
| **浏览器扩展** | Chrome / Edge · Manifest V3 | [Edge 加载项商店](https://microsoftedge.microsoft.com/addons/detail/mkfokebcmknjnbjceabimdchdfhbdhhc) · [源码](https://github.com/EastMG/gacha-calendar-extension) | 已上架 · [Releases](https://github.com/EastMG/gacha-calendar-extension/releases) |
| **PWA / App** | 可安装 PWA（离线可用） | [在线使用](https://eastmg.github.io/gacha-calendar-app/) · [源码](https://github.com/EastMG/gacha-calendar-app) | 已上线 · 三端原生壳待定 |
| **Windows 小组件** | 任务栏常驻 · C# / .NET 10 · WPF | [源码](https://github.com/EastMG/gacha-calendar) | v0.1 · 源码构建 |
| **DSH 插件** | DeepSeek Harness 侧边栏 | [npm](https://www.npmjs.com/package/dsh-gacha-calendar) · [源码](https://github.com/EastMG/dsh-gacha-calendar) | v0.12.5 |
| **共享核心** | 零依赖抓取 / 解析核心（npm） | [gacha-calendar-core](https://www.npmjs.com/package/gacha-calendar-core) | v0.12.5 · 四端共用 |

**设计取舍**：抓取放在客户端 / CI（浏览器受 CORS 限制，Node 没有），用「零服务端 + 近实时」换掉代理服务器；解析器只维护一处，桌面端 / 扩展 / PWA / 插件全部复用核心，不在各端重复实现。

## 🛒 其他在做的

- **[shopping-mcp](https://github.com/EastMG/dsh-shopping-mcp)** — 淘宝 / 京东 / 拼多多 商品搜索、详情、转链接的 MCP server。只调官方开放平台接口，没有凭证时以 mock 模式直接可跑。
- **[millennium-csp-bridge](https://github.com/EastMG/millennium-csp-bridge)** — 让 Millennium 主题与插件脚本在 Steam 商店 / 社区页恢复执行（不关闭 CSP，不改主题）。

## 🧰 常用的

`TypeScript` · `Node.js` · `C# / .NET (WPF)` · `Python` · `Chromium MV3` · `GitHub Actions`

## 📌 最近

- **2026-10** — 新增 `gacha-calendar-app`（PWA 已可安装、离线可用）与 `gacha-calendar`（Windows 任务栏小组件 v0.1）
- **2026-10** — 扩展 v0.2.6、DSH 插件 v0.12.5、共享核心 `gacha-calendar-core` 0.12.5
- PWA 的数据由 GitHub Actions 每 6 小时抓取一轮后重新部署（浏览器受 CORS 限制，Node 没有）

## 🔗 找我

[npm](https://www.npmjs.com/~eastmorning) · [Edge 加载项](https://microsoftedge.microsoft.com/addons/detail/mkfokebcmknjnbjceabimdchdfhbdhhc) · [二游日历 PWA](https://eastmg.github.io/gacha-calendar-app/)

Roadmap：[二游日历 · Roadmap](https://github.com/users/EastMG/projects/1)

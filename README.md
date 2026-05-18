# 📊 RevenueParser

**广告收入数据可视化仪表盘，一目了然掌握收入趋势与广告表现。**

[![在线访问](https://img.shields.io/badge/在线访问-点击体验-blue)](https://aiyangdie.github.io/RevenueParser)

---

## 📌 项目简介

RevenueParser 是一款纯前端广告收入数据可视化仪表盘，专为小程序 / App 广告收入分析设计。通过折线图、饼图、柱状图、堆叠柱状图四种图表，直观呈现总收入趋势、广告类型占比、各类型收入对比及近 7 天收入明细，帮助开发者快速洞察收入数据。

---

## ✨ 核心特性

- 📈 **总收入趋势图** — 折线图展示每日收入变化趋势
- 🥧 **广告类型占比** — 饼图直观展示五大广告类型收入占比
- 📊 **各类型收入对比** — 柱状图横向对比各广告类型总收入
- 📅 **近 7 天收入明细** — 堆叠柱状图展示近一周各广告类型每日收入
- 💰 **汇总数据卡片** — 总收入、日均收入、最高日收入三大核心指标
- 📱 **响应式布局** — Grid 自适应布局，桌面端双列 / 移动端单列
- 🎨 **Material 风格** — 白色卡片 + 圆角阴影，简洁专业

---

## 🛠️ 技术栈

| 技术 | 用途 |
|------|------|
| HTML5 | 页面结构 |
| CSS3 | Grid 布局、响应式设计、卡片样式 |
| JavaScript (ES6+) | 数据处理、图表渲染 |
| [Chart.js](https://www.chartjs.org/) | 图表可视化库（CDN 引入） |

### 支持的广告类型

| 类型 | 英文标识 | 说明 |
|------|----------|------|
| 激励广告 | incentive | 用户观看后获得奖励的广告 |
| 插屏广告 | interstitial | 全屏插页式广告 |
| 原生模板 | native | 与内容融合的原生广告 |
| 封面广告 | cover | 开屏 / 封面式广告 |
| Banner 广告 | banner | 底部横幅广告 |

---

## 🚀 快速开始

### 前置条件

- 现代浏览器（Chrome / Firefox / Edge / Safari）

### 安装步骤

```bash
git clone https://github.com/aiyangdie/RevenueParser.git
cd RevenueParser
```

### 运行

直接在浏览器中打开 `index.html` 即可使用。

### 自定义数据

在 `index.html` 中找到 `rawData` 数组，替换为你的广告收入数据：

```javascript
const rawData = [
    {date: '2025-04-29', total: 0.49, incentive: 0.30, interstitial: 0.07, native: 0.09, cover: 0.02, banner: null},
    // 添加更多数据...
];
```

字段说明：
- `date` — 日期（YYYY-MM-DD）
- `total` — 当日总收入
- `incentive` / `interstitial` / `native` / `cover` / `banner` — 各广告类型收入（无数据填 `null`）

---

## 📂 项目结构

```
RevenueParser/
├── index.html                  # 主页面（含样式、数据、图表逻辑）
├── CNAME                       # GitHub Pages 自定义域名
└── README.md                   # 项目说明
```

---

## 🤝 贡献与许可证

欢迎提交 PR 或 [报告问题](https://github.com/aiyangdie/RevenueParser/issues)！

本项目采用 MIT 开源协议，您可以自由使用、修改和分发。

---

*📊 让广告收入数据一目了然*

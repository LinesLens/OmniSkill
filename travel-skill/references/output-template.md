# 输出模板

攻略生成两个文件：
- `<目的地>-旅游攻略.md` — Markdown 主文档（编辑、版本管理）
- `<目的地>-旅游攻略.html` — HTML 移动端查看器（手机扫码查看，含 QR 码）

---

## 一、Markdown 模板

```markdown
# <目的地>旅游攻略

> 📅 <出行日期> | 🕐 <天数>天 | 👥 <人数>人 | 💰 <预算类型>
> 兴趣：<兴趣偏好列表>

---

## 目录

- [精简概要](#精简概要)
- [详细行程](#详细行程)
- [住宿推荐](#住宿推荐)
- [预算估算](#预算估算)
- [实用信息](#实用信息)

---

## 精简概要

<目的地>简介，3-5 句话概述城市/地区特色、最佳旅行季节和本次行程亮点。

| 日期 | 主题 | 核心活动 | 天气 |
|------|------|---------|------|
| Day 1: <日期> | <主题> | <核心活动> | <天气> |

---

## 详细行程

### Day 1: <日期> — <主题>

#### ⏱ 重大节点时间轴

| 时间 | 类型 | 事件 | 备注 |
|------|------|------|------|
| 🥣 08:30 | 早餐 | <餐厅/菜品> | <备注，如"酒店自助早餐"> |
| 🚇 09:00 | 出行 | <出发前往景点> | <交通方式、耗时> |
| 🎯 10:30 | 景点 | <观看表演/参观> | <建议提前10分钟到场> |
| 🥢 11:30 | 午餐 | <餐厅名> ⭐<大众点评评分> | <必点菜品、预订提示> |
| 🎯 14:00 | 景点 | <活动名称> | <实用提示> |
| 🍖 18:00 | 晚餐 | <餐厅名> ⭐<大众点评评分> | <必点菜品、预订提示> |

#### 🌅 时段安排

| 时段 | 时间 | 活动 | 详情 |
|------|------|------|------|
| 🥣 早餐 | 08:30-09:00 | <餐厅/菜品> | <描述> |
| 🌅 上午 | 09:00-12:00 | <活动名> | <描述，含预估时间和实用提示> |
| 🥢 午餐 | 11:30-13:00 | <餐厅名> ⭐<评分> | <描述，含餐厅推荐、人均、必点菜> |
| ☀️ 下午 | 13:00-17:00 | <活动名> | <描述> |
| 🍖 晚餐 | 18:00-19:30 | <餐厅名> ⭐<评分> | <描述，含餐厅推荐、人均、必点菜、预订提示> |
| 🎯 自由时间 | 19:30+ | 自由探索 | <附近推荐> |

#### 🗺️ 路线地图

[查看路线](<Amap 路线链接，格式：https://ditu.amap.com/dir?from%5Bname%5D=出发地&to%5Bname%5D=目的地>)

#### 🏛️ 景点

**<景点名>**（<当地语言名>）
- 门票：<价格>
- 开放时间：<时间>
- 建议游览：<时长>
- 提示：<游览建议>

![景点名](<已验证图片 URL>)
*📷 示意图 · <具体描述，关联真实景点特征>*

#### 🍜 美食推荐

| 餐厅 | 类型 | 人均 | 大众点评 | 必点 | 地址 | 预订 |
|------|------|------|---------|------|------|------|
| [<餐厅名称>](https://ditu.amap.com/search?query=<餐厅名>%20<城市>) | <类型> | <人均> | ⭐<评分> (<评论数>评) | <必点菜品> | <地址> | <预订提示> |

![美食](<已验证图片 URL>)
*📷 示意图 · <描述>*

#### 🚗 交通建议

<当天交通方式和注意事项>

#### 🌧️ 雨天备选

| 室内活动 | 说明 |
|----------|------|
| <活动名> | <描述> |

---

（每个 Day 重复以上结构）

---

## 住宿推荐

| 酒店 | 区域 | 类型 | 人均/晚 | 大众点评 | 地址 | 优势 |
|------|------|------|---------|---------|------|------|
| [<酒店名称>](https://ditu.amap.com/search?query=<酒店名>%20<城市>) | <区域> | <类型> | <人均/晚> | ⭐<评分> (<评论数>评) | <地址> | <优势> |

---

## 预算估算

| 类别 | 预估费用（人均） | 备注 |
|------|-----------------|------|
| 🚗 大交通 | <金额> | <机票/火车票说明> |
| 🏨 住宿 | <金额> | <按 X 晚计算> |
| 🍜 餐饮 | <金额> | <每日估算> |
| 🎫 门票 | <金额> | <主要景点门票合计> |
| 🚇 市内交通 | <金额> | <交通卡/单次票> |
| 🛍️ 购物 | <金额> | <酌情预估> |
| 📱 其他 | <金额> | <SIM 卡、保险等> |
| **合计** | **<总金额>** | |

---

## 实用信息

### 🌤️ 天气与穿衣

- 出行期间天气趋势：<描述>
- 温度范围：<范围>
- 穿衣建议：<建议>
- 必备物品：<列表>

数据来源：<✅ 实时数据 / 📌 参考数据>

### 🚇 交通卡/通票

| 卡/票名称 | 适用范围 | 价格 | 购买方式 | 性价比 |
|----------|---------|------|---------|--------|
| <名称> | <范围> | <价格> | <方式> | <建议> |

### 🛂 签证信息

- 签证类型：<类型>
- 办理方式：<方式>
- 所需材料：<列表>
- 办理时间：<时长>
- 注意事项：<提示>

数据来源：📌 参考数据，建议出行前向使领馆核实

### 🎎 当地习俗

- <习俗/禁忌 1>
- <习俗/禁忌 2>

### 🗣️ 常用语言

| 中文 | 当地语言 | 发音 |
|------|---------|------|
| 你好 | ... | ... |
| 谢谢 | ... | ... |
| 多少钱 | ... | ... |
| 在哪里 | ... | ... |
| 救命/帮助 | ... | ... |

### 🆘 紧急联系

| 类型 | 电话 | 地址/备注 |
|------|------|----------|
| 报警 | <电话> | |
| 急救 | <电话> | |
| 中国大使馆 | <电话> | <地址> |
| 旅游热线 | <电话> | |

### 📸 拍照打卡点

| 地点 | 最佳时间 | 拍摄建议 |
|------|---------|---------|
| <地点> | <时间> | <建议> |

![拍照点](<Pexels 图片 URL>)

---

## 旅行小贴士

1. **<贴士主题>**：<内容>
2. **<贴士主题>**：<内容>

---

> 📌 本攻略于 <生成日期> 生成，部分信息可能已有变化，建议出行前核实关键信息（航班、酒店、门票价格等）。
```

---

## 二、HTML 查看器模板

用于手机扫码查看，带响应式设计 + QR 码自生成。

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title><目的地>旅游攻略</title>
<style>
  :root {
    --primary: #e8724a;
    --primary-dark: #c05a32;
    --bg: #fdf6f0;
    --card-bg: #ffffff;
    --text: #333333;
    --text-secondary: #666666;
    --text-light: #999999;
    --border: #e8ddd4;
    --border-light: #f0e8dc;
    --accent-gold: #d4a853;
    --tag-bg: #fef3e8;
    --shadow: 0 2px 12px rgba(0,0,0,0.06);
    --radius: 12px;
    --max-width: 900px;
    --ink: #2a3a4a;
    --clay: #c85a32;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
    background: var(--bg); color: var(--text); line-height: 1.8; padding: 0;
    font-size: 17px; -webkit-font-smoothing: antialiased;
  }

  /* ─── HEADER ─── */
  .header {
    background: linear-gradient(135deg, #2a3a4a 0%, #e8724a 100%);
    color: #fff; padding: 48px 20px 40px; text-align: center; position: relative; overflow: hidden;
  }
  .header h1 { font-size: 2.4em; margin-bottom: 10px; letter-spacing: 2px; }
  .header .meta-tags { display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; font-size: 0.9em; opacity: 0.92; margin-top: 12px; }
  .header .meta-tags span { background: rgba(255,255,255,0.15); padding: 4px 12px; border-radius: 100px; }

  /* ─── MAIN ─── */
  .main { max-width: var(--max-width); margin: 0 auto; padding: 0 24px 56px; }

  /* ─── TOC ─── */
  .toc { background: var(--card-bg); border-radius: var(--radius); padding: 28px 32px; box-shadow: var(--shadow); margin-bottom: 28px; }
  .toc h2 { font-size: 1.2em; margin-bottom: 14px; color: var(--primary-dark); }
  .toc-ol { list-style: none; padding: 0; display: grid; grid-template-columns: 1fr 1fr; gap: 4px 20px; }
  .toc-ol li { counter-increment: toc-n; }
  .toc-ol a {
    display: flex; align-items: center; gap: 10px; padding: 8px 12px;
    border-radius: 8px; text-decoration: none; color: var(--text);
    font-weight: 500; font-size: 0.92em; transition: background 0.2s;
  }
  .toc-ol a::before {
    content: counter(toc-n, decimal-leading-zero);
    font-weight: 700; font-size: 0.95em; color: var(--primary-dark); min-width: 24px;
  }
  .toc-ol a:hover { background: #fef3e8; }

  /* ─── SECTIONS ─── */
  .section { background: var(--card-bg); border-radius: var(--radius); padding: 40px 42px; box-shadow: var(--shadow); margin-bottom: 28px; }
  .section h2 { font-size: 1.4em; color: var(--primary-dark); border-bottom: 2px solid var(--border); padding-bottom: 10px; margin-bottom: 20px; }
  .section h3 { font-size: 1.1em; color: #555; margin: 24px 0 12px; }

  /* ─── COLLAPSIBLE DAY CARD ─── */
  .day-card { border: 1px solid var(--border); border-radius: var(--radius); margin-bottom: 24px; overflow: hidden; }
  .day-card[open] .day-hd::after { transform: rotate(180deg); }
  .day-hd {
    background: var(--ink); color: #fff; padding: 16px 22px;
    display: flex; justify-content: space-between; align-items: center;
    font-weight: 600; font-size: 1em; cursor: pointer; list-style: none;
  }
  .day-hd::-webkit-details-marker { display: none; }
  .day-hd::after {
    content: "▾"; font-size: 1.2em; margin-left: 10px; flex-shrink: 0;
    transition: transform 0.3s; opacity: 0.7;
  }
  .day-hd .dh-wx {
    font-size: 0.78em; font-weight: 400;
    background: rgba(255,255,255,0.12); padding: 4px 12px; border-radius: 100px;
  }
  .day-body { padding: 24px; background: var(--card-bg); animation: ds-in 0.25s ease; }
  @keyframes ds-in { from { opacity: 0; transform: translateY(-8px); } to { opacity: 1; transform: translateY(0); } }

  /* ─── BRACKET TIMELINE (ds-r) ─── */
  .ds { display: grid; gap: 10px; margin: 0; }
  .ds-r {
    display: grid; grid-template-columns: 90px 1fr; gap: 10px;
    padding: 12px 16px; border-radius: 10px; font-size: 0.9em; line-height: 1.7;
    border-left: 4px solid var(--border-light); background: #fefaf7;
  }
  .ds-r.meal { border-left-color: var(--clay); background: linear-gradient(90deg, rgba(200,90,50,0.06), rgba(200,90,50,0.01)); }
  .ds-r.transit { border-left-color: #4a6a8a; background: linear-gradient(90deg, rgba(74,106,138,0.05), rgba(74,106,138,0.01)); }
  .ds-r.free { border-left-color: var(--accent-gold); background: linear-gradient(90deg, rgba(212,168,83,0.08), rgba(212,168,83,0.01)); }
  .ds-tm { font-weight: 700; color: var(--primary-dark); font-size: 0.92em; white-space: nowrap; min-width: 65px; }
  .ds-bd strong { display: block; color: var(--ink); margin-bottom: 2px; }
  .ds-bd .ds-note { display: block; font-size: 0.85em; color: var(--text-secondary); margin-top: 2px; }

  /* ─── KEY-TIME BADGE ─── */
  .kt {
    display: inline-block; padding: 2px 9px; border-radius: 100px;
    font-weight: 600; font-size: 0.82em; margin-right: 4px;
  }
  .kt.m { background: #fde8de; color: var(--clay); }    /* meal */
  .kt.t { background: #e8edf4; color: #4a6a8a; }        /* transit */
  .kt.e { background: #faf0d8; color: #7a5f18; }        /* event */

  /* ─── ATTRACTION BOX ─── */
  .abox {
    border-left: 3px solid var(--clay); background: #fefaf7;
    padding: 16px 20px; margin: 16px 0; border-radius: 0 10px 10px 0; font-size: 0.9em;
  }
  .abox h4 { color: var(--clay); font-size: 0.95em; margin-bottom: 4px; }
  .am { display: flex; flex-wrap: wrap; gap: 5px; margin-bottom: 6px; }
  .am em { background: #fef3e8; padding: 2px 9px; border-radius: 100px; font-size: 0.82em; color: var(--text-secondary); font-style: normal; }
  .ai { width: 100%; max-height: 260px; object-fit: cover; border-radius: 8px; margin: 10px 0; border: 1px solid var(--border-light); }

  /* ─── FOOD GRID ─── */
  .fig { display: grid; grid-template-columns: repeat(4, 1fr); gap: 10px; margin: 16px 0; }
  .fig img { width: 100%; height: 120px; object-fit: cover; border-radius: 8px; border: 1px solid var(--border-light); }

  /* ─── TABLES ─── */
  .dt { width: 100%; border-collapse: collapse; font-size: 0.88em; margin: 12px 0; }
  .dt thead th { background: #fef3e8; color: var(--primary-dark); padding: 10px 10px; text-align: left; font-weight: 600; white-space: nowrap; font-size: 0.82em; border-bottom: 2px solid var(--border); }
  .dt tbody td { padding: 10px 10px; border-bottom: 1px solid var(--border-light); vertical-align: top; }
  .dt tbody tr:hover td { background: #fefaf7; }
  .dt a { color: var(--clay); text-decoration: none; font-weight: 600; }
  .dt a:hover { text-decoration: underline; }
  .rating { color: var(--accent-gold); font-weight: 700; white-space: nowrap; }
  .rating-count { font-size: 0.82em; color: var(--text-light); }

  /* ─── MAP LINK ─── */
  .ml { margin: 10px 0 6px; font-size: 0.82em; }
  .ml a { color: var(--clay); text-decoration: none; font-weight: 500; }
  .ml a:hover { text-decoration: underline; }

  /* ─── RAINY ─── */
  .rainy { border: 1px dashed #d0d8e0; background: #f8fafc; border-radius: 10px; padding: 10px 14px; margin-top: 12px; font-size: 0.82em; color: var(--text-secondary); }
  .rainy strong { color: var(--ink); font-weight: 600; }

  /* ─── SOURCE BADGE ─── */
  .sb { display: inline-block; padding: 2px 8px; border-radius: 100px; font-size: 0.72em; font-weight: 500; }
  .sb-ok { background: #e8f5e9; color: #2e7d32; }
  .sb-ref { background: #fff8e1; color: #e65100; }

  /* ─── TIPS ─── */
  .tips-ol { list-style: none; padding: 0; counter-reset: n; }
  .tips-ol li { padding: 10px 0; border-bottom: 1px solid var(--border-light); font-size: 0.87em; counter-increment: n; display: flex; gap: 14px; line-height: 1.7; }
  .tips-ol li::before { content: counter(n, decimal-leading-zero); font-weight: 700; font-size: 1.15em; color: var(--clay); min-width: 32px; flex-shrink: 0; }

  /* ─── BACK TO TOP ─── */
  #btt {
    position: fixed; bottom: 24px; right: 24px; z-index: 60;
    width: 44px; height: 44px; border-radius: 50%;
    background: rgba(255,255,255,0.92); backdrop-filter: blur(12px);
    border: 1px solid var(--border); color: var(--clay);
    font-size: 1.2em; cursor: pointer; display: flex; align-items: center; justify-content: center;
    opacity: 0; transform: translateY(20px); transition: opacity 0.3s, transform 0.3s;
    pointer-events: none; box-shadow: var(--shadow);
  }
  #btt.visible { opacity: 1; transform: translateY(0); pointer-events: auto; }
  #btt:hover { background: #fef3e8; border-color: var(--clay); }

  /* ─── FOOTER ─── */
  .footer { text-align: center; color: var(--text-light); font-size: 0.8em; padding: 24px 0 12px; line-height: 2; }

  /* ─── RESPONSIVE ─── */
  @media (max-width: 740px) {
    .section { padding: 24px 20px; }
    .section h2 { font-size: 1.25em; }
    .day-body { padding: 16px; }
    .ds-r { grid-template-columns: 70px 1fr; font-size: 0.82em; }
    .toc-ol { grid-template-columns: 1fr; }
    .header h1 { font-size: 1.6em; }
    .fig { grid-template-columns: 1fr 1fr; }
  }
  @media (max-width: 480px) {
    .ds-r { grid-template-columns: 60px 1fr; font-size: 0.78em; }
    .ds-tm { min-width: 50px; font-size: 0.8em; }
    .fig { grid-template-columns: 1fr; }
  }
  @media print {
    body { background: #fff; font-size: 14px; }
    .nav-bar, #btt { display: none; }
    .header { background: #2a3a4a !important; -webkit-print-color-adjust: exact; }
    .section { box-shadow: none; break-inside: avoid; border: 1px solid #ddd; }
    .day-hd { background: #2a3a4a !important; -webkit-print-color-adjust: exact; }
  }
</style>
</head>
<body>

<div class="header">
  <h1><目的地>旅游攻略</h1>
  <div class="meta-tags">
    <span>📅 <出行日期></span>
    <span>🕐 <天数>天</span>
    <span>👥 <人数>人</span>
    <span>💰 <预算类型></span>
  </div>
</div>

<div class="main">

<!-- TOC -->
<div class="toc">
  <h2>📋 目录</h2>
  <ol class="toc-ol">
    <li><a href="#overview">精简概要</a></li>
    <li><a href="#itinerary">详细行程</a></li>
    <li><a href="#accommodation">住宿推荐</a></li>
    <li><a href="#restaurants">美食打卡</a></li>
    <li><a href="#budget">预算估算</a></li>
    <li><a href="#info">实用信息</a></li>
    <li><a href="#photospots">拍照打卡</a></li>
    <li><a href="#tips">旅行小贴士</a></li>
  </ol>
</div>

<!-- OVERVIEW -->
<div class="section" id="overview">
  <h2>精简概要</h2>
  <p><目的地简介，3-5 句话></p>
  <table class="dt" style="margin-top:14px;">
    <tr><th>日期</th><th>主题</th><th>核心活动</th><th>天气</th></tr>
    <tr><td>Day 1: <日期></td><td><主题></td><td><核心活动></td><td><天气></td></tr>
  </table>
  <p style="margin-top:10px;font-size:0.78em;color:var(--text-light);"><span class="sb sb-ref">📌 参考</span> 建议出行前查询实时信息</p>
</div>

<!-- ITINERARY -->
<div id="itinerary">

<!-- Day N: 折叠卡片 -->
<details class="day-card" open>
  <summary class="day-hd"><span>Day <N> · <日期> — <主题></span><span class="dh-wx"><天气></span></summary>
  <div class="day-body">

    <!-- 统一左边框时间轴 -->
    <div class="ds">
      <div class="ds-r meal"><div class="ds-tm"><span class="kt m">08:30</span></div><div class="ds-bd"><strong>🥣 早餐：<餐厅/菜品></strong><span class="ds-note"><备注></span></div></div>
      <div class="ds-r transit"><div class="ds-tm"><span class="kt t">09:00</span></div><div class="ds-bd"><strong>🚌 出发/交通</strong><span class="ds-note"><实用提示></span></div></div>
      <div class="ds-r"><div class="ds-tm"><span class="kt e">10:30</span></div><div class="ds-bd"><strong>景点/活动</strong><span class="ds-note"><实用提示></span></div></div>
      <div class="ds-r meal"><div class="ds-tm"><span class="kt m">11:30</span></div><div class="ds-bd"><strong>🥢 午餐：<餐厅名> ⭐<评分></strong><span class="ds-note"><必点菜品></span></div></div>
      <div class="ds-r"><div class="ds-tm"><span class="kt e">14:00</span></div><div class="ds-bd"><strong>下午活动</strong><span class="ds-note"><实用提示></span></div></div>
      <div class="ds-r meal"><div class="ds-tm"><span class="kt m">18:00</span></div><div class="ds-bd"><strong>🍖 晚餐：<餐厅名> ⭐<评分></strong><span class="ds-note"><必点菜品、预订提示></span></div></div>
      <div class="ds-r free"><div class="ds-tm"><span class="kt e">20:00</span></div><div class="ds-bd"><strong>🎯 自由探索</strong><span class="ds-note"><附近推荐></span></div></div>
    </div>

    <!-- 景点详情 -->
    <div class="abox">
      <h4><景点名></h4>
      <div class="am"><em><门票></em><em><建议游览时长></em></div>
      <img class="ai" src="<已验证的图片URL>" alt="<景点名>" loading="lazy">
      <small style="display:block;color:var(--text-light);margin-top:4px">📷 <示意图/实拍> · <具体描述，关联真实景点特征></small>
      <p><景点简介与游览提示></p>
    </div>

    <!-- 地图链接（URL 编码格式） -->
    <p class="ml">🗺️ <a href="https://ditu.amap.com/dir?from%5Bname%5D=<出发地>&to%5Bname%5D=<目的地>" target="_blank">查看路线</a> — <路线简述></p>

    <!-- 雨天备选 -->
    <div class="rainy"><strong>雨天备选</strong> · <室内活动></div>
  </div>
</details>
<!-- 每天重复，Day 1 带 open 属性，其余不带 -->

</div>

<!-- ACCOMMODATION -->
<div class="section" id="accommodation">
  <h2>住宿推荐</h2>
  <table class="dt">
    <tr><th>酒店</th><th>入住</th><th>人均/晚</th><th>评分</th><th>亮点</th><th>地址</th></tr>
    <tr>
      <td><strong><a href="https://ditu.amap.com/search?query=<酒店名> <城市>" target="_blank"><酒店名称></a></strong></td>
      <td><入住日期></td><td><人均价格/晚></td>
      <td><span class="rating">★<评分></span><span class="rating-count">(<评论数>)</span></td>
      <td><优势></td><td><地址></td>
    </tr>
  </table>
</div>

<!-- RESTAURANTS -->
<div class="section" id="restaurants">
  <h2>美食打卡清单</h2>
  <table class="dt">
    <tr><th>餐厅</th><th>日期</th><th>时段</th><th>评分</th><th>必点推荐</th><th>预订</th><th>地址</th></tr>
    <tr>
      <td><strong><a href="https://ditu.amap.com/search?query=<餐厅名> <城市>" target="_blank"><餐厅名称></a></strong></td>
      <td><日期></td><td><span class="kt m">18:00</span> 晚餐</td>
      <td><span class="rating">★<评分></span><span class="rating-count">(<评论数>)</span></td>
      <td><必点菜品></td><td><预订提示></td><td><地址></td>
    </tr>
  </table>
  <div class="fig" style="margin-top:16px;">
    <img src="<已验证美食图片URL>" alt="<菜品1>" loading="lazy">
    <img src="<已验证美食图片URL>" alt="<菜品2>" loading="lazy">
    <img src="<已验证美食图片URL>" alt="<菜品3>" loading="lazy">
    <img src="<已验证美食图片URL>" alt="<菜品4>" loading="lazy">
  </div>
</div>

<!-- BUDGET -->
<div class="section" id="budget">
  <h2>预算估算</h2>
  <table class="dt">
    <tr><th>类别</th><th>预估费用（人均）</th><th>备注</th></tr>
    <tr><td>🚗 大交通</td><td><金额></td><td><说明></td></tr>
    <tr><td>🏨 住宿</td><td><金额></td><td><按 X 晚计算></td></tr>
    <tr><td>🍜 餐饮</td><td><金额></td><td><每日估算></td></tr>
    <tr><td>🎫 门票</td><td><金额></td><td><主要景点></td></tr>
    <tr><td>🚇 市内交通</td><td><金额></td><td><交通方式></td></tr>
    <tr><td>🛍️ 购物</td><td><金额></td><td><酌情预估></td></tr>
    <tr style="font-weight:700;background:#fef3e8;"><td>合计</td><td><strong><总金额></strong></td><td></td></tr>
  </table>
  <p style="font-size:0.78em;color:var(--text-light);"><span class="sb sb-ref">📌 参考</span></p>
</div>

<!-- INFO -->
<div class="section" id="info">
  <h2>实用信息</h2>
  <h3>🌤️ 天气与穿衣</h3>
  <ul class="tips-ol">
    <li><span><天气趋势></span></li>
    <li><span>温度范围：<范围></span></li>
    <li><span>穿衣建议：<建议></span></li>
    <li><span>必备物品：<列表></span></li>
  </ul>
  <p style="font-size:0.82em;color:var(--text-light);">数据来源：<✅ 实时 / <span class="sb sb-ref">📌 参考</span>></p>

  <h3>🚌 当地交通</h3>
  <table class="dt">
    <tr><th>区间</th><th>方式</th><th>耗时</th><th>票价</th><th>购票渠道</th></tr>
    <tr><td><区间></td><td><方式></td><td><耗时></td><td><票价></td><td><渠道></td></tr>
  </table>

  <h3>🎎 当地习俗</h3>
  <ul class="tips-ol">
    <li><span><习俗/注意事项></span></li>
  </ul>

  <h3>🗣️ 常用语言</h3>
  <table class="dt">
    <tr><th>中文</th><th>当地语言</th><th>发音</th></tr>
    <tr><td>你好</td><td>...</td><td>...</td></tr>
    <tr><td>谢谢</td><td>...</td><td>...</td></tr>
  </table>

  <h3>🆘 紧急联系</h3>
  <table class="dt">
    <tr><th>类型</th><th>电话</th><th>备注</th></tr>
    <tr><td>报警</td><td><电话></td><td></td></tr>
    <tr><td>急救</td><td><电话></td><td></td></tr>
  </table>
</div>

<!-- PHOTO SPOTS -->
<div class="section" id="photospots">
  <h2>拍照打卡指南</h2>
  <p style="margin-bottom:12px;font-size:0.9em;">以下为推荐机位与拍摄建议：</p>
  <table class="dt">
    <tr><th>地点</th><th>最佳时间</th><th>拍摄建议</th></tr>
    <tr><td><地点></td><td><时间></td><td><建议></td></tr>
  </table>
</div>

<!-- TIPS -->
<div class="section" id="tips">
  <h2>出行贴士</h2>
  <ol class="tips-ol">
    <li><span><strong><贴士主题></strong>：<内容></span></li>
  </ol>
</div>

<!-- FOOTER -->
<div class="footer">
  <p>📌 本攻略于 <生成日期> 生成，建议出行前 3-5 天核实关键信息（航班、酒店、门票预约）。</p>
</div>

</div>

<script>
// back-to-top button
(function(){
  var btn = document.createElement('button');
  btn.id = 'btt'; btn.innerHTML = '&#8593;'; btn.title = '回到顶部';
  document.body.appendChild(btn);
  function toggle(){ btn.classList.toggle('visible', window.scrollY > 300); }
  btn.addEventListener('click', function(){ window.scrollTo({top:0, behavior:'smooth'}); });
  window.addEventListener('scroll', toggle, {passive: true});
})();
</script>

</body>
</html>
```

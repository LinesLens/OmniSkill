# 小红书卡片模板

> 当用户要求生成小红书截图卡片时加载此文件。所有卡片尺寸 1179×1941px，打开即截图。

## 目录

1. [共用样式 shared.css](#共用样式)
2. [封面卡片模板](#封面卡片)
3. [每日行程卡片模板](#每日行程卡片)
4. [美食合集卡片模板](#美食合集卡片)
5. [预算卡片模板](#预算卡片)
6. [结尾卡片模板](#结尾卡片)
7. [图片规范](#图片规范)
8. [校验清单](#校验清单)

---

## 共用样式

文件 `shared.css` 被所有卡片引用。以下是完整模板（精确字号为实战验证值）：

```css
:root {
  --clay: #C85A32; --clay-d: #A84A2A; --clay-l: #FDF0EA;
  --ink: #1A2533; --ink-l: #3A4A5E;
  --gold: #D4A853; --gold-l: #FAF1E0;
  --cream: #FBF5ED; --white: #FFFEFC;
  --border: #E8DDD4; --border-l: #F0E8DC;
  --text: #1E1A14; --muted: #6B5E4E; --light: #9B8D7A;
  --meal: #C85A32; --transit: #4A6A8A; --event: #D4A853;
  --w: 1179px; --h: 1941px;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

html { background: #E8E0D8; }
body {
  width: var(--w); min-height: var(--h); margin: 0 auto;
  font-family: "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Noto Serif SC", sans-serif;
  color: var(--text); background: var(--white);
  position: relative; -webkit-font-smoothing: antialiased;
}

.card { width: var(--w); min-height: var(--h); position: relative; display: flex; flex-direction: column; }

/* Progress */
.progress { display: flex; gap: 8px; justify-content: center; padding: 28px 0 40px; }
.progress span { width: 10px; height: 10px; border-radius: 50%; background: var(--border); flex-shrink: 0; }
.progress span.active { background: var(--clay); width: 28px; border-radius: 5px; }

/* Signature */
.sig { text-align: center; padding: 12px 0 8px; flex-shrink: 0; font-size: 20px; color: var(--light); letter-spacing: 1px; }

/* Day Header */
.day-header { padding: 80px 80px 0 80px; flex-shrink: 0; display: flex; justify-content: space-between; align-items: flex-start; }
.day-header-left { flex: 1; }
.day-num-watermark { font-size: 200px; font-weight: 900; line-height: 1; color: var(--clay); opacity: 0.07; position: absolute; top: 20px; left: 40px; z-index: 0; pointer-events: none; }
.day-pn { font-size: 28px; font-weight: 700; color: var(--muted); letter-spacing: 3px; white-space: nowrap; padding-top: 14px; flex-shrink: 0; }
.day-label { font-size: 30px; font-weight: 700; color: var(--clay); letter-spacing: 8px; text-transform: uppercase; margin-bottom: 10px; }
.day-title { font-size: 72px; font-weight: 900; color: var(--ink); line-height: 1.1; letter-spacing: -0.5px; }
.day-meta { display: flex; gap: 24px; margin-top: 22px; align-items: center; flex-wrap: wrap; }

/* Tags */
.tag { display: inline-block; padding: 10px 26px; border-radius: 100px; font-size: 22px; font-weight: 600; }
.tag-wx-s { background: #FEF6E8; color: #C97A20; }
.tag-wx-c { background: #EEF2F8; color: #4A6290; }

/* Timeline */
.timeline { display: flex; flex-direction: column; gap: 16px; padding: 40px 80px 0 80px; flex-shrink: 0; }
.tl-row { display: grid; grid-template-columns: 120px 1fr; gap: 20px; align-items: start; padding: 22px 28px; border-radius: 16px; border-left: 6px solid var(--border-l); background: #fefaf7; font-size: 28px; line-height: 1.6; }
.tl-row.meal { border-left-color: var(--meal); background: linear-gradient(90deg, rgba(200,90,50,0.05), rgba(200,90,50,0.01)); }
.tl-row.transit { border-left-color: var(--transit); background: linear-gradient(90deg, rgba(74,106,138,0.05), rgba(74,106,138,0.01)); }
.tl-row.free { border-left-color: var(--gold); background: linear-gradient(90deg, rgba(212,168,83,0.06), rgba(212,168,83,0.01)); }
.tl-time { font-weight: 700; color: var(--clay-d); font-size: 30px; white-space: nowrap; }
.tl-body strong { display: block; color: var(--ink); margin-bottom: 4px; font-size: 28px; }
.tl-body .tl-note { font-size: 22px; color: var(--muted); }

/* Badges */
.kt { display: inline-block; padding: 6px 18px; border-radius: 100px; font-weight: 700; font-size: 22px; }
.kt.m { background: #FDE8DE; color: var(--clay-d); }
.kt.t { background: #E8EDF4; color: #4A6A8A; }
.kt.e { background: var(--gold-l); color: #7A5F18; }

/* Attraction */
.attr { padding: 40px 80px; flex-shrink: 0; display: grid; grid-template-columns: 1fr 1fr; gap: 40px; }
.attr-img { width: 100%; height: 480px; object-fit: cover; border-radius: 16px; border: 1px solid var(--border-l); }
.attr-info h4 { font-size: 40px; color: var(--clay-d); margin-bottom: 16px; }
.attr-info p { font-size: 26px; color: var(--muted); line-height: 1.8; }
.attr-meta { display: flex; flex-wrap: wrap; gap: 12px; margin: 16px 0; }
.attr-meta em { background: var(--clay-l); padding: 8px 22px; border-radius: 100px; font-size: 20px; color: var(--muted); font-style: normal; }
.img-cap { display: block; font-size: 19px; color: var(--light); margin-top: 10px; }

/* Rainy */
.rainy { margin: 0 80px; padding: 18px 28px; flex-shrink: 0; border: 1px dashed #D0D8E0; background: #F8FAFC; border-radius: 12px; font-size: 22px; color: var(--muted); }
.rainy strong { color: var(--ink); }

/* Cover */
.cover-content { position: relative; z-index: 2; display: flex; flex-direction: column; align-items: center; justify-content: center; height: 1941px; padding: 80px; color: #fff; text-align: center; }
.cover-tagline { font-size: 28px; font-weight: 500; letter-spacing: 10px; color: var(--gold); margin-bottom: 24px; text-transform: uppercase; }
.cover-title { font-size: 108px; font-weight: 900; line-height: 1.05; letter-spacing: -1px; margin-bottom: 28px; }
.cover-hook { font-size: 52px; font-weight: 700; margin-bottom: 20px; background: linear-gradient(135deg, #FFD89B, #FF8A5C); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; }
.cover-sub { font-size: 26px; opacity: 0.8; margin-bottom: 40px; line-height: 1.6; }
.cover-tags { display: flex; flex-wrap: wrap; justify-content: center; gap: 16px; margin-bottom: 48px; }
.cover-tags span { background: rgba(255,255,255,0.12); backdrop-filter: blur(8px); padding: 12px 28px; border-radius: 100px; font-size: 24px; font-weight: 600; }
.cover-footer { font-size: 22px; opacity: 0.6; }

/* Ending */
.ending-quote { font-size: 68px; font-weight: 900; color: var(--ink); line-height: 1.25; margin-bottom: 48px; }
.ending-stats { display: flex; gap: 44px; margin-bottom: 60px; }
.ending-stat { text-align: center; }
.ending-stat .num { font-size: 80px; font-weight: 900; color: var(--clay); line-height: 1; }
.ending-stat .label { font-size: 22px; color: var(--muted); margin-top: 8px; }
.ending-cta { font-size: 36px; font-weight: 700; color: var(--ink); margin-bottom: 20px; }
.ending-cta-sub { font-size: 24px; color: var(--muted); margin-bottom: 48px; }
.cta-box { display: inline-block; background: var(--clay); color: #fff; padding: 22px 56px; border-radius: 100px; font-size: 30px; font-weight: 700; box-shadow: 0 8px 32px rgba(200,90,50,0.3); }

/* Food */
.food-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; padding: 0 80px 32px 80px; flex-shrink: 0; }
.food-card { display: flex; gap: 20px; padding: 24px; border-radius: 16px; background: var(--white); border: 1px solid var(--border-l); align-items: center; }
.food-card img { width: 130px; height: 130px; object-fit: cover; border-radius: 12px; flex-shrink: 0; }
.food-card h4 { font-size: 26px; margin-bottom: 4px; color: var(--ink); }
.food-card .fc-day { font-size: 18px; color: var(--clay); margin-bottom: 6px; font-weight: 600; }
.food-card .fc-dish { font-size: 20px; color: var(--muted); }
.food-card .fc-price { font-size: 19px; color: var(--light); margin-top: 4px; }

/* Budget */
.bar-row { display: grid; grid-template-columns: 160px 1fr 130px; gap: 24px; align-items: center; margin-bottom: 20px; }
.bar-label { font-size: 28px; font-weight: 600; color: var(--ink); text-align: right; }
.bar-track { height: 48px; background: #f0ebe2; border-radius: 100px; overflow: hidden; }
.bar-fill { height: 100%; border-radius: 100px; display: flex; align-items: center; justify-content: flex-end; padding-right: 20px; font-size: 22px; font-weight: 700; color: #fff; min-width: 80px; }
.bar-amount { font-size: 28px; font-weight: 700; color: var(--clay-d); }
```

---

## 封面卡片

文件 `01-cover.html`。深色背景 + 大图蒙层 + SVG 路线图。

```html
<!DOCTYPE html><html lang="zh-CN"><head><meta charset="UTF-8"><title>封面</title>
<link rel="stylesheet" href="shared.css"><style>
  body{background:#1A2533}
  .cover-bg-img{position:absolute;inset:0;background:url('<风景图URL>') center/cover no-repeat}
  .cover-overlay-strong{position:absolute;inset:0;background:linear-gradient(180deg,rgba(26,37,51,0.15) 0%,rgba(26,37,51,0.65) 50%,rgba(26,37,51,0.92) 100%)}
  .hero-icon{font-size:90px;margin-bottom:20px}
  .divider{width:100px;height:4px;background:var(--gold);margin:36px auto;border-radius:2px}
  .route-map{margin:40px auto 0;width:950px;height:240px;opacity:0.9}
  .bottom-bar{position:absolute;bottom:100px;left:0;right:0;text-align:center;z-index:3}
</style></head><body>
<div class="card">
  <div class="cover-bg-img"></div>
  <div class="cover-overlay-strong"></div>
  <div class="cover-content" style="position:relative;z-index:2">
    <div class="hero-icon">🏔️</div>
    <div class="cover-tagline"><目的地英文> · <年份></div>
    <div class="cover-title"><目的地></div>
    <div class="cover-hook"><天数>天<N>晚 · 人均 ¥<金额></div>
    <div class="divider"></div>
    <div class="cover-sub"><一句话描述></div>
    <div class="cover-tags"><span>景点1</span><span>景点2</span>...</div>
    <!-- SVG 路线图：金→粘土渐变虚线，起点✈️+终点⭐，5-6个标记点 -->
  </div>
  <div style="position:absolute;bottom:130px;left:0;right:0;text-align:center;z-index:3;font-size:16px;color:rgba(255,255,255,0.35)">📷 封面背景来自图库，非实拍</div>
  <div class="bottom-bar"><div class="cover-footer"><日期> · <人数> · <风格></div></div>
  <div class="sig" style="position:relative;z-index:3;color:rgba(255,255,255,0.4)">@AiBytes</div>
  <div class="progress" style="position:relative;z-index:3"><span class="active"></span><span></span>...共12个</div>
</div></body></html>
```

---

## 每日行程卡片

文件 `02-day1.html` ~ `09-day8.html`。统一模板：

```html
<!DOCTYPE html><html lang="zh-CN"><head><meta charset="UTF-8"><title>Day N</title>
<link rel="stylesheet" href="shared.css"><style>body{background:linear-gradient(180deg,#FBF5ED 0%,#FFFEFC 40%,#FFFEFC 100%)}</style></head><body>
<div class="card">
  <div class="day-num-watermark">0N</div>
  <div class="day-header">
    <div class="day-header-left">
      <div class="day-label">DAY N · M/D</div>
      <div class="day-title"><主题></div>
      <div class="day-meta"><span class="tag tag-wx-s">☀️ 晴 20-35°C</span><span style="font-size:18px;color:var(--muted)">交通方式</span></div>
    </div>
    <div class="day-pn">0N/12</div>
  </div>
  <div class="timeline">
    <div class="tl-row meal"><div class="tl-time"><span class="kt m">08:00</span></div><div class="tl-body"><strong>🥣 早餐</strong><span class="tl-note">描述</span></div></div>
    <div class="tl-row transit"><div class="tl-time"><span class="kt t">09:00</span></div><div class="tl-body"><strong>🚌 交通</strong><span class="tl-note">描述</span></div></div>
    <div class="tl-row"><div class="tl-time"><span class="kt e">11:00</span></div><div class="tl-body"><strong>📍 景点</strong><span class="tl-note">描述</span></div></div>
    <div class="tl-row meal"><div class="tl-time"><span class="kt m">11:30</span></div><div class="tl-body"><strong>🥢 午餐</strong><span class="tl-note">餐厅 · 人均</span></div></div>
    <div class="tl-row free"><div class="tl-time"><span class="kt e">20:00</span></div><div class="tl-body"><strong>🎯 自由探索</strong><span class="tl-note">描述</span></div></div>
  </div>
  <div class="attr">
    <div><img class="attr-img" src="<已验证Pexels URL>" alt="<景点>" loading="lazy"><span class="img-cap">📷 <景点> · <实用提示></span></div>
    <div class="attr-info"><h4>🏛️ <景点名></h4><div class="attr-meta"><em>🎫 <价格></em><em>⏱ <时长></em></div><p><描述></p></div>
  </div>
  <div class="rainy"><strong>🌧️ 雨天备选</strong> · <室内活动></div>
  <div class="sig">@AiBytes</div>
  <div class="progress"><span></span><span class="active"></span>...</div>
</div></body></html>
```

**关键规则**：
- 每张卡片 5-8 个 `.tl-row`，分类使用 `.meal` / `.transit` / `.free`
- `.tl-row` 不使用 `flex: 1`，全部 `flex-shrink: 0`，内容紧密排列
- 时间徽章 `.kt` 三类：`.kt.m`（用餐）、`.kt.t`（交通）、`.kt.e`（活动）
- 配图 Pexels URL 须 `curl -sI` 验证 HTTP 200
- 最后一天（Day 8）也必须有配图

---

## 美食合集卡片

文件 `10-food.html`。暖色背景，8 格餐厅：

```html
<!DOCTYPE html><html lang="zh-CN"><head><meta charset="UTF-8"><title>美食合集</title>
<link rel="stylesheet" href="shared.css"><style>body{background:linear-gradient(180deg,#FBF5ED 0%,#FFFEFC 40%,#FFFEFC 100%)}</style></head><body>
<div class="card">
  <div style="padding:60px 80px 28px;text-align:center;flex-shrink:0;position:relative">
    <div style="font-size:24px;color:var(--clay);letter-spacing:8px;margin-bottom:10px">XINJIANG CUISINE</div>
    <div style="font-size:68px;font-weight:900;color:var(--ink);margin-bottom:10px">🍖 跟着吃就对了</div>
    <div style="font-size:24px;color:var(--muted)">8家本地人推荐的老店，都帮你试过了</div>
    <div style="position:absolute;top:60px;right:100px;font-size:28px;font-weight:700;color:var(--muted);letter-spacing:3px">10/12</div>
  </div>
  <div class="food-grid">
    <div class="food-card"><img src="<URL>" alt="<菜>" loading="lazy"><div><h4><餐厅名></h4><div class="fc-day">Day N · ⭐4.6</div><div class="fc-dish"><必点></div><div class="fc-price">人均 ¥30-50</div></div></div>
    <!-- 重复8次 -->
  </div>
  <div style="text-align:center;padding:12px 80px 0;flex-shrink:0;font-size:24px;color:var(--muted)">每个本地人推荐的老店，都帮你试过了 ✨</div>
  <div class="sig">@AiBytes</div>
  <div class="progress"><span></span>...共12个</div>
</div></body></html>
```

---

## 预算卡片

文件 `11-budget.html`。横向条形图 + 省钱 tips：

```html
<!DOCTYPE html><html lang="zh-CN"><head><meta charset="UTF-8"><title>预算一览</title>
<link rel="stylesheet" href="shared.css"><style>body{background:linear-gradient(180deg,#FBF5ED 0%,#FFFEFC 100%)}</style></head><body>
<div class="card">
  <div class="budget-header">
    <div class="bh-label">BUDGET BREAKDOWN</div>
    <div class="bh-title">💰 钱都花哪了</div>
    <div class="bh-sub">人均预算估算</div>
  </div>
  <div class="total-badge"><div class="tb-num">¥3,700</div><div class="tb-label">人均总预算 · 含往返机票</div></div>
  <div class="bars-section">
    <div class="bar-row"><div class="bar-label">✈️ 往返机票</div><div class="bar-track"><div class="bar-fill c1">¥1,200-1,500</div></div><div class="bar-amount">最大头</div></div>
    <!-- 重复6行：住宿/门票/交通/餐饮/购物 -->
  </div>
  <div class="tips-section"><h4>💡 省钱 Tips</h4><span class="tip-row">...</span></div>
  <div class="sig">@AiBytes</div>
  <div class="progress"><span></span>...</div>
</div></body></html>
```

---

## 结尾卡片

文件 `12-ending.html`。情感金句 + 数据回顾 + CTA：

```html
<!DOCTYPE html><html lang="zh-CN"><head><meta charset="UTF-8"><title>结尾</title>
<link rel="stylesheet" href="shared.css"><style>
  body{background:linear-gradient(180deg,#FBF5ED 0%,#1A2533 100%)}
  .ending-bg-img{position:absolute;inset:0;background:url('<URL>') center/cover no-repeat;opacity:0.18}
</style></head><body>
<div class="card">
  <div class="ending-bg-img"></div>
  <div style="position:relative;z-index:2;display:flex;flex-direction:column;align-items:center;justify-content:center;height:1941px;padding:80px 100px;text-align:center">
    <div style="font-size:22px;color:var(--gold);letter-spacing:6px;margin-bottom:20px">THANK YOU FOR READING</div>
    <div class="ending-quote"><金句></div>
    <div class="ending-stats"><div class="ending-stat"><div class="num">8</div><div class="label">天</div></div></div>
    <div class="ending-cta">你最想打卡哪个景点？</div>
    <div class="ending-cta-sub">评论区告诉我 👇</div>
    <div class="cta-box">快分享给你的旅行搭子吧 🧳</div>
    <div style="font-size:28px;margin-top:36px;letter-spacing:3px">#<span style="color:var(--clay);font-weight:700">北疆伊犁</span> ...</div>
  </div>
  <div class="sig" style="position:relative;z-index:3">@AiBytes</div>
  <div class="progress" style="position:relative;z-index:3"><span></span>...共12个</div>
</div></body></html>
```

---

## 图片规范

1. **Pexels 优先**：因 CDN 连通性最佳，所有配图使用 Pexels
2. **URL 验证**：每张图片写入 HTML 前必须 `curl -sI --max-time 5 "<URL>"` 验证 HTTP 200
3. **Caption 格式**：`📷 <景点描述> · <实用提示>`（如 `📷 赛里木湖 · 湖水湛蓝，风大带冲锋衣`）
4. **禁用"示意图"字样**：实战验证此标注在小红书会触发"非原创"判定
5. **封面和结尾**：大图做背景 + 蒙层，不单独展示
6. **美食卡片**：8 张不同图片，不用重复素材

---

## 校验清单

小红书卡片输出前确认：

- [ ] 14 个文件全部生成（shared.css + 12 卡片 + index.html）
- [ ] 每张卡片 body 精确 1179×1941px，html 背景 #E8E0D8，body margin: 0 auto
- [ ] 所有图片 URL 通过 curl -sI 验证 HTTP 200
- [ ] 封面含 SVG 路线图（6 个标记点，金→粘土渐变虚线）
- [ ] 每张卡片底部有 `<div class="sig">@AiBytes</div>` 签名
- [ ] 配图 caption 格式：`📷 景点描述 · 实用提示`（不含"示意图"字样）
- [ ] 评分使用 ⭐ 格式
- [ ] 餐厅和酒店名称附带可点击 Amap 搜索链接
- [ ] 美食卡片背景与其他卡片一致（暖色系 `#FBF5ED→#FFFEFC`）
- [ ] 所有卡片使用 `flex-shrink: 0`，无弹性空白
- [ ] 字体仅使用系统字体，不加载 Google Fonts
- [ ] 字号与参考值一致（72px / 28px / 40px / 26px / 22px...）
- [ ] 像素值使用 px 单位，不使用 em/rem/vw

# AI Agent 成果展示網站

這是一個展示「國立臺北科技大學創新研究與技術發展成長社群 - AI Agent 使用者經驗研究與產品開發」社群成果的一頁式網站。

## 專案資訊

- **社群名稱**：AI Agent 使用者經驗研究與產品開發
- **召集人**：陳靜儀
- **學院系所**：設計學院工業設計系
- **活動期間**：2025年5月1日 - 2025年12月31日
- **參與學生**：10 位
- **工作坊場次**：6 場

## 網站特色

### 🎨 設計風格
- **現代科技感**：深色主題搭配 AI 風格的藍紫色漸層
- **動態背景**：浮動的漸層光球，隨滑鼠移動產生互動效果
- **玻璃擬態**：半透明背景與模糊效果
- **流暢動畫**：滾動觸發的淡入動畫、卡片懸浮效果

### 📱 響應式設計
- 支援桌面、平板、手機等不同螢幕尺寸
- 自適應網格佈局

### 🚀 互動功能
- 平滑滾動導航
- 滾動觸發動畫
- 滑鼠互動背景
- 專案卡片 3D 傾斜效果
- 視差滾動效果

## 網站結構

### 1. Hero Section（主視覺區）
- 全螢幕動態背景
- 社群標題與資訊
- 召集人與學院系所資訊
- CTA 按鈕

### 2. About Section（社群介紹）
- 活動期間
- 參與成員統計
- 工作坊場次
- 成果產出

### 3. Timeline Section（活動時間軸）
6 場工作坊活動：
1. 領域驅動設計與UX設計師的角色貢獻（07/14）
2. LLM 的下一步？從 Agent 聊聊 Agentic AI（07/15）
3. Agent 實作工作坊（07/22 上午）
4. 領域驅動設計與UX設計師的角色貢獻工作坊 II（07/22 下午）
5. Google AI 生態系（08/17）
6. 生成式AI 產品開發社群成果發表（09/02）

### 4. Projects Section（學生作品展示）
10 位學生的作品：
1. **Civitas Watch** - 李宣諺
2. **VoteAI** - 劉承璟
3. **Task Mapper** - 林瑞苓
4. **PromptWeaver** - 劉陶樺
5. **Heartfelt Picks** - 邱彥仁
6. **LexiPedia** - 董岱靈
7. **GenKit** - 陳宜晗
8. **Bullshit Master & 說故事大師** - 張家熏
9. **IdeaForge** - 馮筱芸
10. **FINDFOOD** - 張紫蘭

每個作品卡片包含：
- 產品介紹圖片
- 學生姓名
- 作品名稱
- 簡短描述
- 查看簡報連結

## 如何使用

### 本地預覽

1. 開啟終端機，進入專案目錄：
```bash
cd /Users/ching-macmini/.gemini/antigravity/scratch/ai-agent-showcase
```

2. 啟動本地伺服器：
```bash
python3 -m http.server 8000
```

3. 在瀏覽器開啟：
```
http://localhost:8000
```

### 檔案結構

```
ai-agent-showcase/
├── index.html          # 主頁面
├── styles.css          # 樣式表
├── script.js           # 互動腳本
├── assets/             # 資源目錄
│   ├── students/       # 學生作品圖片（10張）
│   └── activities/     # 活動照片（預留）
└── README.md           # 使用說明
```

## 技術棧

- **HTML5**：語意化標籤
- **CSS3**：
  - CSS Variables（設計系統）
  - Flexbox & Grid（佈局）
  - Animations & Transitions（動畫）
  - Backdrop Filter（玻璃擬態）
  - Gradients（漸層效果）
- **JavaScript（Vanilla）**：
  - Intersection Observer API（滾動動畫）
  - Mouse Event（互動效果）
  - Smooth Scroll（平滑滾動）

## 自訂修改

### 更新活動照片
將活動照片放入 `assets/activities/` 目錄，然後在 `index.html` 中對應的活動區塊加入圖片：

```html
<div class="timeline-photos">
    <img src="assets/activities/activity-1.jpg" alt="活動照片">
</div>
```

### 修改配色
在 `styles.css` 的 `:root` 區塊修改 CSS 變數：

```css
:root {
    --color-primary: #00d4ff;      /* 主色 */
    --color-secondary: #8b5cf6;    /* 次要色 */
    --color-accent: #00ff88;       /* 強調色 */
}
```

### 更新學生資訊
在 `index.html` 中找到對應的 `.project-card` 區塊，修改內容即可。

## 瀏覽器支援

- Chrome（推薦）
- Firefox
- Safari
- Edge

## 授權

© 2025 國立臺北科技大學. All rights reserved.

---

**建立日期**：2025年11月21日  
**建立工具**：Antigravity AI

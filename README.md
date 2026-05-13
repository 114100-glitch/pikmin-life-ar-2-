# 🌱 Pikmin Life AR

> 現實世界 AR 冒險遊戲 — Web PWA 版本

## ✨ 功能

- 📷 **AR 相機** — 開啟後背相機，Pikmin 出現在現實世界中
- 🗺️ **GPS 健走** — 走路自動累積步數、金幣，每 30 步召喚 Pikmin
- 📖 **圖鑑系統** — 9 種 Pikmin（普通/稀有/超稀有/傳說）
- 👾 **世界 Boss** — 與其他玩家合力擊倒 Boss
- 🧠 **生物題庫** — 答題獲得獎勵
- ⭐ **VIP 系統** — VIP1/VIP2 提升倍率
- 🎁 **每日獎勵** — 連續簽到提升獎勵
- 🏰 **公會系統** — 加入公會一起冒險
- 🎫 **兌換碼** — 支援特殊碼兌換金幣

## 🚀 GitHub Pages 部署步驟

### 第一步：建立 GitHub Repository

1. 前往 https://github.com/new
2. Repository name 填入：`pikmin-life-ar`
3. 設為 **Public**
4. 點擊 **Create repository**

### 第二步：上傳檔案

```bash
# 在你的電腦上執行：
git init
git add .
git commit -m "🌱 Initial commit - Pikmin Life AR"
git branch -M main
git remote add origin https://github.com/你的帳號/pikmin-life-ar.git
git push -u origin main
```

### 第三步：開啟 GitHub Pages

1. 進入你的 Repository
2. 點擊上方 **Settings**
3. 左側選單找 **Pages**
4. Source 選擇 **GitHub Actions**
5. 等待 1-2 分鐘，網址會出現：
   `https://你的帳號.github.io/pikmin-life-ar`

### 第四步：手機加到主畫面（PWA）

**iPhone：** Safari 打開網址 → 分享 → 加入主畫面  
**Android：** Chrome 打開網址 → 右上角選單 → 安裝應用程式

---

## 🎫 內建兌換碼

| 兌換碼 | 獎勵 |
|--------|------|
| `VIP0102` | 60,000 金幣 |
| `PIKMIN2024` | 10,000 金幣 |
| `WELCOME` | 5,000 金幣 |

---

## 📱 手機權限說明

- **相機** — AR 功能需要後鏡頭
- **位置** — GPS 步數追蹤需要

---

## 📁 檔案結構

```
pikmin-life-ar/
├── index.html          # 主遊戲檔案（全部功能）
├── manifest.json       # PWA 設定
├── sw.js               # Service Worker（離線支援）
├── icon-192.png        # App 圖示 192x192
├── icon-512.png        # App 圖示 512x512
└── .github/
    └── workflows/
        └── deploy.yml  # 自動部署腳本
```

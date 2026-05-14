# joshhu.github.io

胡嘉璽 Josh Hu 的個人形象網頁原始碼 — AI 應用專家、暢銷書作家、企業 AI 導入顧問。

🌐 **線上版本**：
- 主站：[josh.hu](https://josh.hu/)（GitHub Pages，本 repo 自動部署）
- 鏡像：[keen-halo-524w.here.now](https://keen-halo-524w.here.now/)（here.now 同步發佈）

## 特色

- **單檔 HTML**：所有 CSS / JS 內嵌於 `index.html`，無建置流程，無框架依賴
- **深色科技風**：青藍 × 紫 × 粉霓虹漸層，Hero 動態粒子背景 + 滑鼠跟隨光暈
- **豐富互動**：打字機效果、Scroll Reveal 進場、3D 卡片傾斜、數字計數動畫、Konami code 彩蛋
- **響應式佈局**：桌機 4 欄書牆 → 平板 3 欄 → 手機 1 欄
- **真實內容**：7 本博客來著作真封面（連商品頁可購買）+ 6 大企業 AI 課程模組

## 目錄結構

```
.
├── index.html                       # 主頁面（內含 CSS / JS）
├── profile.jpg                      # Hero 區個人形象照
├── covers/
│   └── 1.jpg ~ 7.jpg                # 博客來書籍封面
├── CNAME                            # GitHub Pages 自訂網域 (josh.hu)
├── googleb14e638a0e558dea.html      # Google Search Console 驗證
└── README.md
```

> 歷史備註：此 repo 原為 Hexo 部落格「在範式間穿梭」(2014–2017)，原始檔保留於 [`hexo-archive`](https://github.com/joshhu/joshhu.github.io/tree/hexo-archive) 分支。

## 技術堆疊

| 類別 | 使用 |
|---|---|
| 結構 | HTML5 |
| 樣式 | 純 CSS（自訂屬性 + Grid + backdrop-filter） |
| 互動 | Vanilla JavaScript（IntersectionObserver、Canvas 粒子、3D tilt） |
| 字型 | Noto Sans TC、Space Grotesk、JetBrains Mono（Google Fonts） |
| 部署 | GitHub Pages（josh.hu）+ [here.now](https://here.now/) 鏡像 |

## 區塊

1. **Hero** — 名字、職業 tag、打字機輪播、雙 CTA、雙軌道行星動畫頭像
2. **About / Stats** — 自我介紹、技術棧 14 項、4 個關鍵數字（100+ 著作、500+ 場演講、20000+ 學員、35 年經驗）
3. **Publications** — 7 本暢銷書 + 1 張「100+ 本」摘要卡，皆連博客來
4. **Enterprise AI Courses** — 6 大課程模組（戰略 / 開發 / 治理）+ 4 步驟合作流程
5. **Why Choose Me** — 4 大差異化優勢
6. **Quote** — 「AI 不會取代您的員工，但會用 AI 的員工會」
7. **Contact** — Facebook / Email / 博客來連結 + 30 分鐘免費諮詢 CTA

## 本機預覽

直接用瀏覽器開 `index.html` 即可，或起一個簡易 server：

```bash
python3 -m http.server 8000
# 開啟 http://localhost:8000
```

## 部署

### GitHub Pages（主站 josh.hu）

```bash
git add -A
git commit -m "<變更說明>"
git push origin master
# GitHub Pages 自動重建，1-2 分鐘後 josh.hu 生效
```

`CNAME` 檔（內容 `josh.hu`）必須保留於根目錄，否則自訂網域會解除綁定。

### here.now（鏡像 keen-halo-524w）

```bash
# 安裝 here.now skill（一次性）
npx skills add heredotnow/skill --skill here-now -g

# 部署 / 更新
bash ~/.agents/skills/here-now/scripts/publish.sh . --slug keen-halo-524w
```

需要 here.now API key 才能更新既有的永久站點，存於 `~/.herenow/credentials`。

## 著作 / 課程聯絡

- 📘 著作：[博客來作者頁](https://search.books.com.tw/search/query/key/%E8%83%A1%E5%98%89%E7%92%BD/adv_author/1/)
- 📧 Email：joshhu.usa@gmail.com
- 👤 Facebook：[胡嘉璽 Josh Hu](https://www.facebook.com/profile.php?id=61579313407097)

## License

© 2026 胡嘉璽 Josh Hu。內容（文案、形象照、書封）保留所有權利；網頁原始碼結構供學習參考。

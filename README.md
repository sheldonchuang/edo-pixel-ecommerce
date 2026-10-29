# 熱血江戶一番街 (Retro 8-Bit Edo Street Gamified E-Commerce)

> 結合「任天堂紅白機《熱血物語》復古風格」與「江戶時代 3D 街景購物」的遊戲化電商原型。

---

## 🎮 遊戲與操作說明

- **移動**：`W` `A` `S` `D` 或 方向鍵（2.5D 軸側橫向捲軸視角，可上下移動深淺）
- **調查 / 交談 / 購物**：走近町屋商店或 NPC 按 `E` 鍵或 `Enter`
- **熱血拳擊**：按 `空白鍵 (Space)` 或 `J` 鍵。街上的木箱可以擊碎，有機會掉落金幣或 **88折折價券（EDO88）**！
- **行囊錢袋**：點擊右上角購物車圖示可查看所選商品、套用折價代碼並進行交割（下單結帳）。
- **觸控支援**：手機或平板開啟時自動呈現復古虛擬方向鍵與 A/B 互動按鈕。

---

## 🛠️ 技術特點

- **純前端單檔架構**：以原生 HTML5 + Three.js (ES Module) + Tailwind CSS 打造，無任何編譯負擔。
- **真 8-Bit 像素化渲染**：
  - 低原生解析度渲染 + CSS `image-rendering: pixelated` 保持純粹像素顆粒感。
  - 材質貼圖全面採用 `THREE.NearestFilter`。
  - 復古硬邊陰影（`THREE.BasicShadowMap`）與 CRT 掃描線濾鏡。
- **純程式 8-Bit 音效**：內建 Web Audio API 音頻合成器，無須外載音檔即有逼逼聲、打擊音效與金幣聲。

---

## 🚀 部署至 Render.com (100% 免費靜態網站)

本專案已配置 `render.yaml` 藍圖，部署至 Render 為 **永久免費 Static Site**（不休眠、全球 CDN 加速）：

1. 登入 [Render.com](https://render.com/)。
2. 點擊右上角 **New +** ➔ 選擇 **Static Site**。
3. 連結您的 GitHub 儲存庫（`edo-pixel-ecommerce`）。
4. 設定參數：
   - **Name**: `edo-pixel-ecommerce`（或自訂）
   - **Branch**: `main`
   - **Build Command**: 留空（不需構建）
   - **Publish Directory**: `.`（當前目錄）
5. 點擊 **Create Static Site**，約 30 秒內即可獲得公開試玩網址！

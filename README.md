# privacy-factory-site

隱私工廠 Privacy Factory 行銷網站(單頁靜態,繁中/English 雙語)。部署於 Vercel。

- **App Store:** 尚未上架(TODO:上架後把 `index.html` 內三處 `href="#"` 換成 https://apps.apple.com/app/id{APP_STORE_ID})
- **隱私權政策 / 使用條款:** https://vincent615.github.io/privacy-factory-legal/
- **支援:** finexam.support@gmail.com

## 結構

- `index.html` — 全站單檔(內聯 CSS + 原生 JS 中英切換,`localStorage` key:`pf-lang`)
- `images/` — 目前為空;截圖先以 CSS 灰卡佔位。之後放入 icon、favicon 與截圖(`{home,template,redact,report}_{zh,en}.jpg`)並把佔位 `.ph` 換回 `<img>`

## 品牌色(曜石黑金,系列第 4 色)

`--bright:#F0CE6A` / `--gold:#D9A62E` / `--amber:#B8860B` / `--bronze:#6B4E14` / `--obsidian:#17120A`

## 系列站連結

Footer 連到掃描/壓縮/轉換工廠(預設 `*.vercel.app` 網址,綁定自訂網域後更新)。

## 本機預覽

```bash
python3 -m http.server 8799
# 開 http://localhost:8799/
```

## 部署(Vercel)

靜態站無 build:Vercel 匯入此 repo → Framework Preset 選 Other → 部署。

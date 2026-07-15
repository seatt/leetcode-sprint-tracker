# LeetCode 衝刺追蹤 - GitHub Pages 版

這是可直接部署到 GitHub Pages 的靜態版追蹤器。

## 一鍵部署到 GitHub

### 方法 1：最快 (3分鐘)

1. 去 GitHub 建一個新 repo，名字例如 `leetcode-sprint-tracker`，設 Public
2. 把這個資料夾裡的檔案全部上傳：
   - `index.html`
   - `assets/` 資料夾
3. 去 Repo 的 **Settings → Pages**
   - Source 選 `Deploy from a branch`
   - Branch 選 `main` / `root` → Save
4. 等 1 分鐘，會給你一個 `https://你的帳號.github.io/leetcode-sprint-tracker/` 連結，分享給朋友就行

### 方法 2：用 git 指令

```bash
git init
git add .
git commit -m "Add LeetCode tracker"
git branch -M main
git remote add origin https://github.com/你的帳號/leetcode-sprint-tracker.git
git push -u origin main
```

然後同樣去 Settings → Pages 開啟。

## 特性

- 純前端，無後端，localStorage 存進度
- 75題真題，Top 20 高頻標記
- Day 1 鎖定模式：先過 #1 和 #3 才解鎖
- 含 Python 模板一鍵複製
- 繁體中文介面

## 自訂

所有題目在 `assets/*.js` 裡被打包了，如果要改題目，建議從原始碼改：
原始碼在 Hatch 的 `ts-spaces/leetcode/client/src/data/problems.ts`

但這個版本可以直接用，不用改就能分享。

## 授權

MIT，自用分享隨意。

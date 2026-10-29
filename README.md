# 邮票类型抢答 · 5 秒一题

看 6 张邮票照片，判断它是 **特种邮票 / 纪念邮票 / 普通邮票**，每题限时 5 秒。

## 怎么部署到 GitHub Pages

1. 打开 https://github.com/new ，仓库名填 `stamp-quiz`，选 **Public**，点 Create repository。
2. 进入仓库 → **Add file → Upload files** → 把本文件夹里的 `index.html` 和 `.nojekyll` 一起拖进去 → Commit changes。
3. 仓库 **Settings → Pages** → Source 选 **Deploy from a branch**，Branch 选 `main` + `/ (root)` → Save。
4. 等 1 分钟，访问：`https://<你的用户名>.github.io/stamp-quiz/`

## 文件说明

- `index.html`：单文件版，6 张邮票图已 base64 内嵌，无外部依赖，离线可用。
- `.nojekyll`：告诉 Pages 不要用 Jekyll 处理这个仓库，避免静态资源被忽略。

## 改题库

`index.html` 里搜 `QUESTIONS` 数组，每题一行：`answer: 'J' | 'T' | 'R'`（纪念 / 特种 / 普通）。

# 每周访谈简报

中美知名对话访谈 / 播客一周精华 · AI 发展 · 前沿科学 · 财经金融 · 宏观 · 地缘

在线访问：<https://raylee710.github.io/>

## 说明

- 纯静态站点，无需构建，`index.html` 直接打开（经 HTTP 访问）。
- `data/weeks.json` 为周索引，最新周排第一。
- 周数据以 `data/<周起始日期>.json.gz.txt`（gzip + base64）形式部署，浏览器端用 `DecompressionStream` 解压；原始 JSON 保留在本地项目 `data/` 目录。
- 嘉宾头像已压缩为 128px JPEG 并内嵌于 `assets/avatars.js`，无需二进制图片文件。
- 本地预览：项目根目录 `node serve.js` 或 `npm run dev`。

## 每周更新

1. 本地 `data/` 新增该周 JSON，并把该周 prepend 到 `data/weeks.json`。
2. 运行 `python build_deploy.py` 重新生成 `_deploy/`。
3. 将 `_deploy/` 内容推送到本仓库 main 分支，GitHub Pages 自动更新。

# Card Ledger — 部署到 GitHub Pages

## 文件清单
- `index.html` — 主 app
- `sw.js` — Service Worker（离线缓存）
- `manifest.json` — PWA 配置
- `icon.png` — 主屏幕图标

## 部署步骤

### 1. 创建 GitHub 仓库
去 github.com → New repository → 名字随意（如 `card-ledger`）→ Public → Create

### 2. 上传文件
把这 4 个文件全部上传到仓库根目录（直接拖进去或 Add file → Upload files）

### 3. 开启 GitHub Pages
仓库页面 → Settings → Pages → Source 选 **main branch / root** → Save

等 1-2 分钟，你会得到一个链接：
`https://你的用户名.github.io/card-ledger/`

### 4. 添加到手机主屏幕（iOS）
1. 用 Safari 打开上面的链接
2. 点底部分享按钮 ↑
3. 选「添加到主屏幕」
4. 确认 → 完成

之后从主屏幕打开就是全屏 App 模式，数据存在手机本地，关掉再开不会丢。

### Android
Chrome 打开链接 → 右上角菜单 → 「添加到主屏幕」

## 数据说明
数据存在浏览器 localStorage，同一台手机不会丢。
换手机或清除浏览器数据会丢失。如需备份，后续可升级到 Supabase 云存储。

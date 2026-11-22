# 滑坡运动过程动力模拟 · 动态演示页

论文补充材料的最小 GitHub Pages 页面，用于给评委提供一个可点击、可扫码的在线动画链接。

## 文件

- `index.html` — 单文件页面，无外部依赖
- `flow.gif` — Bingham 流变模型动画（6.4 MB）
- `voellmy.gif` — Voellmy 流变模型动画（4.5 MB）
- `.nojekyll` — 告诉 GitHub Pages 不要用 Jekyll 处理

## 部署步骤

### 1. 在 GitHub 创建仓库

打开 <https://github.com/new>：

- Repository name：`landslide-animation`（可自定义，会出现在网址里）
- Visibility：**Public**（免费账号的 GitHub Pages 需要公开仓库）
- 不要勾选 “Add a README file”

### 2. 推送本地文件

```bash
cd ~/paper-animation-site
git remote add origin git@github.com:ljingxi154-code/landslide-animation.git
git push -u origin main
```

如果提示没有权限，改用 HTTPS：

```bash
git remote set-url origin https://github.com/ljingxi154-code/landslide-animation.git
git push -u origin main
```

### 3. 开启 Pages

仓库页面 → **Settings** → 左侧 **Pages**：

- Source：**Deploy from a branch**
- Branch：**main** / **/(root)**
- 点击 **Save**

等待 1–2 分钟，页面地址为：

```
https://ljingxi154-code.github.io/landslide-animation/
```

动画直链（用于论文超链接 / 二维码）：

```
Bingham（Pages）：https://ljingxi154-code.github.io/landslide-animation/flow.gif
Voellmy（Pages）：https://ljingxi154-code.github.io/landslide-animation/voellmy.gif
Bingham（raw）  ：https://raw.githubusercontent.com/ljingxi154-code/landslide-animation/main/flow.gif
Voellmy（raw）  ：https://raw.githubusercontent.com/ljingxi154-code/landslide-animation/main/voellmy.gif
```

## 注意

- GitHub Pages 在国内访问可能较慢或不稳定。如果评委主要在国内，建议同时部署到 Gitee Pages 或阿里云 OSS，或把 B 站/腾讯视频作为备用链接。
- 首次打开需要下载 6.4 MB，之后浏览器会缓存。
- 页面点击画面可全屏，右上角可下载 GIF。

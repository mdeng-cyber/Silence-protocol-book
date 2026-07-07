# 静默协议 · 朋友试读版

单文件网页版《静默协议》（朋友试读版，非投稿稿件）。全部 CSS / JS 内联，无任何外部依赖，可直接部署到 GitHub Pages。

## 目录结构

```
silent-protocol/
├── index.html    # 正文（原文件重命名而来）
├── .nojekyll     # 关闭 GitHub 的 Jekyll 处理，避免特殊文件被忽略
└── README.md
```

## 部署方式（三选一）

### 方式 A：网页上传（最简单，无需命令行）

1. 在 GitHub 新建一个仓库，例如 `silent-protocol`
2. 点击 **Add file → Upload files**，把 `index.html` 和 `.nojekyll` 拖进去，提交
3. 进入 **Settings → Pages**
4. Source 选 **Deploy from a branch**，Branch 选 `main` + `/ (root)`，保存
5. 等 1 分钟，页面地址为 `https://<用户名>.github.io/silent-protocol/`

### 方式 B：命令行

```bash
cd silent-protocol
git init
git add .
git commit -m "publish 静默协议 朋友试读版"
git branch -M main
git remote add origin https://github.com/<用户名>/silent-protocol.git
git push -u origin main
```

推送后同样进入 **Settings → Pages** 开启（步骤同方式 A 第 3-5 步）。

### 方式 C：用户主页（根域名访问）

把仓库命名为 `<用户名>.github.io`，`index.html` 放根目录，开启 Pages 后
即可用 `https://<用户名>.github.io/` 直接访问。

## 备注

- 页面为纯静态，手机与桌面自适应，含深浅色切换、阅读进度、水印等原有功能
- 若想改书名，编辑 `index.html` 里的 `<title>` 即可
- 原文件含版权声明与数字指纹水印，请勿外传或用于模型训练

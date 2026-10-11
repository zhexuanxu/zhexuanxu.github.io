# Zhexuan Xu — Academic Homepage

英文科研个人主页，目标网址：**https://zhexuanxu.github.io/**。

## 本地预览

在本站目录运行：

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

浏览器打开 http://127.0.0.1:8000/。也可以直接打开 `index.html`。

## 文件说明

- `index.html`：个人简介、教育经历、论文、荣誉和联系方式。
- `assets/style.css`：配色、字体、布局以及移动端样式。
- `assets/images/`：个人照片及两篇论文配图。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。
- `QA.md`：响应式、内容、链接和可访问性验收记录。
- `docs/`：桌面、平板和手机预览截图。

网页采用纯 HTML/CSS，所有页面资产均保存在本地，无需安装依赖或执行构建。更新论文和个人信息时，直接编辑 `index.html` 即可。

## 部署到 GitHub Pages

1. 在 GitHub 登录 **zhexuanxu** 账号，并检查是否已有 `zhexuanxu.github.io` 仓库。
2. 没有仓库时，新建公开仓库 `zhexuanxu.github.io`。已有仓库时，先保存其历史和现有文件，再更新本站文件。
3. 将本站目录内的文件放到仓库 `main` 分支根目录，确保 `index.html`、`assets/` 和 `.nojekyll` 在同一层级。
4. 打开仓库 **Settings → Pages**，选择 **Deploy from a branch**，分支选 **main**，目录选 **/ (root)**，保存。
5. 等待 Pages 构建成功，然后访问 https://zhexuanxu.github.io/。

使用命令行部署前，可运行 `gh auth status` 检查登录状态。如需重新登录，运行以下命令；认证步骤由账号本人完成：

```sh
gh auth login --hostname github.com --git-protocol https --web
```

GitHub 官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## 资料与配图来源

- 个人资料、照片、导师链接、Scholar 链接和荣誉由徐哲轩提供。
- WideSeek-R1 标题与完整作者顺序：https://wideseek-r1.github.io/
- VS-Bench 标题、完整作者顺序与 CVPR 2026 Oral 状态：https://vs-bench.github.io/
- WideSeek-R1 配图：https://zelaix.github.io/images/publications/wideseek-r1.png
- VS-Bench 配图：https://zelaix.github.io/images/publications/vs-bench.png

两篇论文均保留原作者顺序，徐哲轩为第二位共同第一作者；加粗姓名及星号表示共同一作。论文配图采用原图，网页通过 CSS 缩放完整展示。

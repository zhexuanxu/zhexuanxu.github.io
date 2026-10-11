# 个人主页验收记录

验收日期：2026-10-11。站点采用纯 HTML/CSS；浏览器检查使用 Codex 内置浏览器。

## 响应式与图片

| 视口宽度 | 实测页面宽度 | 结果 |
| --- | --- | --- |
| 375px | 375px | 单列布局，无横向溢出 |
| 768px | 768px | 简介与照片并排，论文左图右文，无横向溢出 |
| 1440px | 1440px | 内容最大宽度 1040px，无横向溢出 |

三张图片均成功加载。个人照片保留脸部和生日帽；两张论文图片使用 `object-fit: contain` 完整显示，保持原始 16:9 比例。

截图：

- [桌面布局](docs/preview-desktop.jpg)
- [平板布局](docs/preview-tablet.jpg)
- [手机布局](docs/preview-mobile.jpg)

## 内容与链接

- 四个导航锚点均有对应区块；实际点击 About 和 Awards 跳转正常。
- 两篇论文均保留完整作者顺序；加粗姓名均为 `Zhexuan Xu*`。
- WideSeek-R1 的前三位作者带共同一作星号，VS-Bench 的前两位作者带共同一作星号。
- 每篇论文显示 Paper、Code、Project Page 三个资源链接。
- 邮箱链接为 `mailto:zx-xu26@mails.tsinghua.edu.cn`；电话链接为 `tel:+8613671000114`。检查链接格式，不触发邮件发送或电话拨打。
- Google Scholar 使用用户指定的 `GsOMCKcAAAAJ` 主页。
- 教育经历按时间倒序展示；中文项目名保留在括号内。
- 实际联网检查的两个导师主页、两个论文页、两个代码页、两个项目页以及少年班学院主页均返回 HTTP 200。
- Google Scholar 对自动请求返回 HTTP 403；已核对链接参数，保留用户指定主页，未改用其他学者页面。

## 可访问性

- 文档语言 `en`，中文项目名称标记 `lang="zh-CN"`。
- 页面具有单一 H1、按层级排列的标题、主导航标签和全部图片替代文本。
- 键盘首次 Tab 到达 Skip to content，Enter 将焦点移动到主内容；再次 Tab 到达导师链接。
- 焦点具有可见的 outline。
- 实测正文对比度 7.80:1；作者、导航和联系方式次要文字对比度 4.59:1；Oral 白字与蓝色背景对比度 6.35:1。
- 尊重 `prefers-reduced-motion`，提供基本打印样式。

## 页面元信息

已配置网页标题、description、canonical URL、Open Graph 信息、favicon 和 `.nojekyll`。网页使用本地样式与图片，不依赖外部字体或脚本。

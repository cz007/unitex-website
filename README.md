# Unitex 官网

Unitex 静态网站，通过 GitHub Pages 发布。

## 页面地址

- [首页](https://unitex-group.github.io/unitex-website/unitex.html)
- [质量页](https://unitex-group.github.io/unitex-website/quality.html)
- [网站根网址](https://unitex-group.github.io/unitex-website/) 会跳转到首页。

## 网站文件

- `unitex.html`：网站首页。
- `quality.html`：质量页面。
- `index.html`：根网址跳转页。
- `assets/`：页面图片和字体。
- `og-image.webp`：首页和质量页的分享预览图。

首页和质量页在 HTML 中设置了各自的 Open Graph 分享标题、简介和网址。卡片效果以微信客户端的转发显示为准。

## 发布

推送到 `main` 后，GitHub Actions 将上述文件复制到 Pages 发布目录。

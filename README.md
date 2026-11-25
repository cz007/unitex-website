# Unitex 官网

公开站点仓库：GitHub Pages + GitHub Actions。

## 页面地址

- 首页：https://cz007.github.io/unitex-website/unitex.html
- 根网址会从 index.html 自动跳转到 unitex.html
- 质量页：https://cz007.github.io/unitex-website/quality.html

## 微信分享卡片

工作流为首页和质量页分别写入 Open Graph 标题、描述、规范 URL 和预览图。预览图片由 og-image.webp.b64 解码生成。微信抓取和缓存由微信侧控制，页面元数据配置好后仍需在微信中实际发送链接确认卡片效果。

## 首页资源

原始 HTML 内嵌图片、字体等数据。为适配网页端上传限制，源文件拆成 site-parts/part-*.txt，工作流会按顺序组装成 unitex.html 和 quality.html。

页面里的 328 个 __UNITEX_ASSET_n__ 标识由内嵌资源脚本解析，并非缺失资源。

## 发布

仓库 Pages 来源为 GitHub Actions。推送到 main 后自动部署。

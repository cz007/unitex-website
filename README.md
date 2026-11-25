# Unitex 公司官网

此仓库托管 Unitex 静态官网，并通过 GitHub Actions 发布到 GitHub Pages。

## 首页资源

首页来自用户提供的 `Unitex.html`，页面内嵌了图片、字体等资源数据。为适配 GitHub 网页端上传限制，HTML 分成 `site-parts/part-*.txt` 多个文本片段；部署工作流会按文件名顺序拼回 `_site/index.html` 再发布。

页面源文件包含 328 个 `__UNITEX_ASSET_n__` 资源标识，由页面内嵌的离线资源脚本解析。这些标识不是缺失资源。

## 发布

仓库 Pages 来源设为 GitHub Actions。推送到 `main` 或从 Actions 手动运行 `Deploy Unitex website to GitHub Pages` 会重新部署。

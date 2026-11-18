# Kaiwen Xue's academic homepage

Website: <https://kaiwenxue.top/>

Repository: <https://github.com/kaiwenxue0/KevinYc5.github.io>

## Files and editing

- `index.html`: biography, publication list, links, and awards. All main content is in the HTML and works without JavaScript.
- `style.css`: responsive homepage layout, mobile styles, keyboard focus, and print styles.
- `publications.bib`: citation records for the four conference papers and one preprint on the homepage.
- `picture/myself.jpg`: existing profile photograph.
- `CNAME`: existing custom domain; keep its contents unchanged.
- `_config.yml`: GitHub Pages metadata.

The original personal statement pages and their stylesheets are retained. The updated homepage uses its own stylesheet so these older pages are unaffected.

To add a paper, duplicate an `<article class="publication">` in the appropriate section of `index.html`, use a unique title ID, update the authors, venue, year and resource links, and add its record to `publications.bib`. Keep peer-reviewed papers and preprints in their respective sections. Update the footer date when editing the content.

## Preview

Open `index.html` directly in a browser, or serve this directory with Python:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000/>. No JavaScript packages or compilation are required.

## Publish to the existing GitHub Pages site

Copy the updated `index.html`, `style.css`, `publications.bib`, `_config.yml`, and `README.md` into the existing repository root, then commit and push to the branch already used by GitHub Pages. Keep `CNAME`, the verification file, and the existing image paths. There is no need to change DNS or create a new Pages site.

The repository's default branch was `master` when this update was prepared. Check the configured Pages publishing branch in GitHub before pushing if it differs from the default. Wait for the Pages deployment to finish, then check <https://kaiwenxue.top/>.

## Content sources (checked 2026-11-18)

- Biography, contact details, degree and awards: original homepage; removed the outdated first-year designation.
- RADD (ICLR 2025): <https://arxiv.org/abs/2406.03736>, <https://openreview.net/pdf?id=0dcMmg0v1l>, <https://github.com/ML-GSAI/RADD>.
- BFN-Solver (ICML 2024): <https://proceedings.mlr.press/v235/xue24d.html>; equal-contribution notation retained from the original homepage.
- UniDiffuser (ICML 2023): <https://arxiv.org/abs/2303.06555>, <https://github.com/thu-ml/unidiffuser>.
- U-ViT (CVPR 2023): <https://arxiv.org/abs/2209.12152>, <https://github.com/baofff/U-ViT>.
- Latent reasoning survey (arXiv 2025): <https://arxiv.org/abs/2507.06203>, <https://arxiv.org/html/2507.06203v2>.

The survey is listed as a preprint; no conference acceptance is claimed. The publication list is not presented as an exhaustive bibliography. No new service roles, awards, or unpublished work have been inferred.

## 中文使用说明

1. 解压后双击 `index.html` 可直接预览，图片和样式无需联网加载。
2. 发布时只需更新仓库根目录的五个文件：`index.html`、`style.css`、`publications.bib`、`_config.yml`、`README.md`。
3. 在 GitHub 仓库中使用 **Add file → Upload files** 上传这五个文件。确认提交到当前 GitHub Pages 使用的分支后，等待 Pages 部署完成。
4. 保留原来的 `CNAME`、Google 验证文件和 `picture/` 目录；域名无需重新配置。
5. 此版本已更新简介，补充 RADD（ICLR 2025）和潜在推理综述（arXiv 2025），完善代码链接、移动端排版和 BibTeX 下载。

此文件包仅表示更新已制作完成，不代表已经提交 GitHub 或发布到线上。

# Homepage design

## Vincent's direction, 2026-11-15

Use [Hayyoth's homepage](https://hayyoth.org/) as a layout reference. Keep Vincent's background pure white. Show contact destinations as labeled hyperlinks: GitHub, Email and Instagram. Preserve the single HTML file, Times New Roman and short personal introduction.

## Reference evidence

Reviewed on 2026-11-15 using Firecrawl markdown, HTML and branding extraction, the original page source, and a browser screenshot. The screenshot was inspected in the chat; no reference image is bundled with the site.

The original CSS sets a 650px centered body, 12px padding, a `#fcefcf` background and `#044c9f` links. Its centered header has a short introduction and a wrapping row of labeled links. Topic links follow in another wrapping row, then a bordered chronology table. Times New Roman is the observed browser font; the original page does not declare a font family.

The highlighted “Opinions on AI” link points to a [YouTube playlist](https://youtube.com/playlist?list=PLbewqW53hsQY). The scrape returned playlist titles alongside an embedded 401 error; video contents were not reviewed and no further access was attempted. Vincent clarified that he wants the layout adapted. No personal opinions were added.

## Implementation choices

| Role | Value |
| --- | --- |
| Background | `#fff`, Vincent's explicit preference |
| Text | `#111` |
| Links | `#044c9f`, underlined |
| Typeface | `"Times New Roman", Times, serif` |
| Body | Browser default size, `1.5` line height |
| Container | `40rem` maximum content width, `1rem` side padding |
| Heading | `2rem`, `1.2` line height |
| Rules | `#aaa` below the header, `#ddd` between projects |

Center the introduction and contact row. Keep the project directory left aligned, with one short description per link. Use a semantic list instead of a chronology table because the content describes projects. The contact row wraps on narrow screens. Links retain native behavior and a visible keyboard focus outline. No scripts, external fonts, imagery or build dependencies are needed.

The existing Kolam Ikan deployment returned HTTP 404 during verification, so its project link now opens the public source repository. Notionpull's existing deployment returned HTTP 200.

## Project description evidence

Public sources were cloned and inspected under `/Users/vincent/core_repos/TOOLS/Gh-Oss/`; no dependencies or project scripts were run from those clones.

- [demucs-mlx README](https://github.com/adittamavincent/demucs-mlx/blob/main/README.md), lines 3–14: Vincent maintains a fork; the tool separates music into stems on Apple Silicon.
- [Splice Tab README](https://github.com/adittamavincent/splice-tab/blob/main/README.md), lines 13–17: desktop sample browsing and previewing.
- [Notionpull README](https://github.com/adittamavincent/notion-pull/blob/main/README.md), lines 1–3: fetching Notion pages and databases and exporting selected content.
- [Kolam Ikan metadata](https://github.com/adittamavincent/kolam-ikan/blob/main/src/app/layout.tsx), lines 19–22: a personal thinking environment and logbook with evolving documentation.

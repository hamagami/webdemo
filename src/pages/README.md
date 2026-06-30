# src/pages

実運用では、このディレクトリでURL構造を決めます。

例:

```text
src/pages/index.astro
src/pages/programs/[slug].astro
src/pages/news/[slug].astro
src/pages/videos/index.astro
```

`content/` のデータを読み込み、URLごとのHTMLを静的生成します。


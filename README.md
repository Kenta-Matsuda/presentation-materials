# presentation-materials

過去の登壇資料をまとめたリポジトリです。GitHub Pages で公開しています。

## 構成

```
index.html                 # 入り口ページ（スライド一覧）
YYYY_MM/<スライド名>/index.html   # 各スライド（Marp で HTML 書き出し）
YYYY_MM/<スライド名>/assets/      # スライドが参照する画像
```

## スライドの追加手順

1. Marp でスライドを HTML に書き出し、`YYYY_MM/<スライド名>/index.html` に置く。
   画像は HTML に埋め込まれないので、参照している `assets/` 以下の画像も同じ相対パスでコピーする。
2. ルートの `index.html` の該当年の `<ol class="talks">` に `<li>` を新しい順で追加する。

## GitHub Pages の設定

リポジトリの Settings → Pages で、Source を「Deploy from a branch」、Branch を `main` / `/ (root)` に設定します。
`.nojekyll` を置いているため、Jekyll の処理は行われずファイルがそのまま配信されます。

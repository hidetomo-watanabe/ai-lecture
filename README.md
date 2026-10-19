# ai-lecture

「現場のAI」（合同会社WhatHides）のLPです。GitHub Pages で公開しています。

公開URL: https://ai-lecture.whathides.co.jp/

## ディレクトリ構成

```
ai-lecture/
├── index.html      ← LP本体（HTML・デモ用JS・構造化データ・GAタグ）
├── css/
│   └── lp-main.css ← LPのスタイル
├── favicon.svg / favicon.ico / apple-touch-icon.png
├── robots.txt
├── sitemap.xml
└── CNAME           ← カスタムドメイン設定
```

## 計測

Google Analytics（`G-DTBNSN6CPC`）を導入しています。
申し込み導線（メールアプリ・Gmail・アドレスコピー）のクリックは `generate_lead` イベントとして送信され、`method` パラメータ（`email` / `gmail` / `copy`）で経路を区別できます。

## GitHub Pages の設定

1. リポジトリの **Settings → Pages**
2. Source を `Deploy from a branch` に設定
3. Branch: `main`、フォルダ: `/ (root)` を選択して Save

## ページを追加するとき

`sitemap.xml` に URL を追加してください。

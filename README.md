# whathides-site

WhatHides サイト一式。GitHub Pages でそのまま公開できます。

## ディレクトリ構成

```
whathides-site/
├── index.html          ← 元のメインHP（既存ファイルをここに置く）
├── store/
│   └── index.html      ← 店舗向けLP
│                          URL: /store/ または /store/index.html
├── css/
│   ├── common.css      ← 共通変数・ナビ・フッター
│   └── lp-store.css    ← 店舗LP専用スタイル
└── js/
    └── (共通JSが必要になったらここに追加)
```

## URL構成

| ページ | URL |
|--------|-----|
| メインHP | `https://<username>.github.io/<repo>/` |
| 店舗向けLP | `https://<username>.github.io/<repo>/store/` |

## 新しいLP（業種別）を追加するには

```
mkdir <業種名>
# 例: manufacturing/, consulting/
```

`store/index.html` をコピーして、コピーとCSS参照パスを調整するだけです。

```html
<!-- store/ の場合 -->
<link rel="stylesheet" href="../css/common.css">
<link rel="stylesheet" href="../css/lp-store.css">
```

## GitHub Pages の設定

1. リポジトリの **Settings → Pages**
2. Source を `Deploy from a branch` に設定
3. Branch: `main`、フォルダ: `/ (root)` を選択して Save

## 既存の index.html を移行する際の注意

既存メインHPのCSSに `common.css` と変数名が衝突する場合は、
`common.css` の変数名（`--c-*`）を任意の名前に変更してください。

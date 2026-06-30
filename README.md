# GitベースCMS プロトタイプ

このディレクトリは、横浜国立大学理工学部Webサイトのリニューアルを想定した、Git管理型CMS運用の小さなプロトタイプです。

## 目的

- コンテンツをGitHubリポジトリ内のファイルとして管理する
- ニュース、学科・EP、動画、画像参照をデータ化する
- Pull Requestでレビューし、mainにマージ後に自動公開する運用を想定する
- 静的サイト生成によって、公開HTMLを作る

## ディレクトリ構造

```text
git-cms-prototype/
├─ index.html
├─ content/
│  ├─ news/
│  ├─ programs/
│  └─ videos/
├─ src/
│  ├─ pages/
│  └─ components/
└─ .github/
   └─ workflows/
```

## 見方

`index.html` をブラウザで開くと、Git管理されたコンテンツから生成される想定のトップページ、EP比較、動画ライブラリ、運用フローを確認できます。

実運用では、`content/` 以下のJSON/Markdown/YAMLを編集し、Pull Requestでレビューした後、GitHub Actionsで静的サイトを生成・公開します。


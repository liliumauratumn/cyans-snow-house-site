# Cyan's Snow House 紹介サイト

Steamで無料公開されている短編ゲーム「Cyan's Snow House（シアンとゆきのいえ）」の
日本語向け公式紹介1ページサイトです。素のHTML/CSSのみで構成され、ビルド工程はありません。

## ファイル構成

```
/
├── index.html
├── README.md
└── assets/
    └── cyan1.png
```

## ローカル確認方法

```
python3 -m http.server 8000
```

ブラウザで `http://localhost:8000` を開いて確認してください。

## GitHubへpush

```
git init
git add .
git commit -m "Create Cyan's Snow House landing page"
git branch -M main
git remote add origin https://github.com/liliumauratumn/cyans-snow-house-site.git
git push -u origin main
```

## Vercelでの公開手順

1. Vercelにログインし、GitHubリポジトリ `cyans-snow-house-site` をImportする
2. Framework Presetは **Other** を選択する
3. ビルドコマンドは不要（空欄のままでよい）
4. 出力ディレクトリの指定も不要
5. Deployを実行する
6. 以後、`main` ブランチへのpushで自動的に再デプロイされる
7. 公開後はVercelから割り当てられた `.vercel.app` のURLを使用する

# ツクロアのウェブサイトのボイラープレート

## 動かし方

### npmパッケージをインストールする

```
$ yarn
```

### ローカルサーバーを立てて開発する

```
$ yarn dev
```

### デプロイ用にビルドする

```
$ yarn build
```

## GitHubワークフロー

### CI

PR時にリントとコード整形します

### Preview

PR時にCloud Runでプレビュー環境を作成します

デフォルトではすべてのブランチで実行しない、かつ、 `env.PROJECT` が空欄なので、利用する場合はコメントアウトされているイベントトリガーに差し替え `env.PROJECT` を設定してください

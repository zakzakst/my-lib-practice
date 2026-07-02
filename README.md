# my-lib-practice

- これ終わったらMonorepoも挑戦してみる

## メモ
- typescriptの最新版6.0.3だと、おそらくtsupとの兼ね合いでエラーが発生したため、一旦npm install -D typescript@5.9を利用している
- package.jsonのfiles設定
  - npm に公開する場合は、files が配布対象を決定します。
  - GitHub リポジトリから直接インストールする場合は、Git リポジトリそのものを取得するため、files だけでは不要なファイルは除外されません。
  - 「じゃあ意味がないの？」いいえ、むしろ今のうちに files を設定しておくのがおすすめです。将来npm Packageへ移行するときにそのまま使えるからです。

## コマンド

```
git commit -m "Release v1.0.0" --allow-empty
git tag v1.0.0
git tag // 設定を確認
git push origin main
git push origin v1.0.0
```

```
npm pack
```
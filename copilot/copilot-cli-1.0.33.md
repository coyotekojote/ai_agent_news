## コマンドエイリアスの追加

`/bug`、`/continue`、`/release-notes`、`/export`、`/reset`、`/upgrade` のコマンドショートカットが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## スマートコマンドサジェスト

スラッシュコマンドピッカーで認識できないコマンドやミスタイプされたコマンドを入力した際に、類似コマンドが提案されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## リモートセッション再開の改善

`--resume` または `--continue` でリモートセッションを再開する際に `--remote` フラグが自動的に引き継がれ、再指定が不要になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## サブエージェントのモデル継承

auto モードのサブエージェントがセッションモデルを継承するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## 使用量制限の早期警告

レート制限に達する前に 50% および 95% の容量警告が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## キーボードショートカットのドキュメント化

`/help` および `?` オーバーレイに Ctrl+T（推論表示の切り替え）、j/k（Vim スタイルナビゲーション）、x（タスクキル）のキーボードショートカットが記載された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

## バグ修正

- コンテンツ除外ポリシーが有効な大規模リポジトリで grep がタイムアウトする問題を修正
- 非対話モードでバックグラウンドエージェントの完了を待機してから終了するよう修正
- スキルピッカーで CJK/日本語の説明や長いスキル名が正しくトランケートされるよう修正
- スラッシュコマンドピッカーで Enter キー押下時にハイライトされたコマンドが選択されるよう修正

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.33)

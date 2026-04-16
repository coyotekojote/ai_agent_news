## Git サブモジュール内での権限プロンプト修正

Git サブモジュール内で作業している際に、権限プロンプトが正しいリポジトリパスを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## バックグラウンドエージェント完了通知の重複排除

`read_agent` が既に結果を待機している場合に、バックグラウンドエージェントの完了通知が重複して表示されないようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## MCP マイグレーションガイダンスの改善

MCP マイグレーションのヒントが、コマンドを直接埋め込む代わりにプラットフォーム固有のドキュメントへリンクするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## Azure リソース ID の誤検知修正

`az` CLI コマンド実行時に Azure リソース ID がパスセキュリティ警告として誤検知されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## Rewind ピッカーのナビゲーション簡素化

Rewind ピッカーのナビゲーションが矢印キーと Enter に簡素化され、紛らわしい数値クイックセレクト機能が削除された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## エディタ起動失敗時のエラーメッセージ改善

設定されたエディタの起動に失敗した際に、明確なエラーメッセージが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## CLI リモートコントロールセッション対応

CLI リモートコントロールセッションへの接続が resume ピッカーからアクセス可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

## その他の改善

- マスコットの起動時の動作が連続的な点滅から短い点滅シーケンスに変更された
- `COPILOT_DISABLE_TERMINAL_TITLE` 環境変数でターミナルタイトル更新の無効化に対応
- `/clear` や `/new` の後にカスタム指示とスキルがディスクから再読み込みされるようになった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.28)

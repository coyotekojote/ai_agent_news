## カスタムテーマのスキーマ修正

カスタムテーマテキストスキーマに不足していた `response` キーが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25822)

## 自動アップデート失敗時の手動コマンド提示

自動アップデートが失敗した場合に手動アップデートコマンドが表示されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26052)

## ECONNRESET・ETIMEDOUT のエラーメッセージ改善

ECONNRESET および ETIMEDOUT 条件に対するエラーメッセージが改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26059)

## サンドボックスプロキシのクリーンアップとハンドラーリーク修正

サンドボックスプロキシのクリーンアップが確実に行われ、ハンドラーリークが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26065)

## JetBrains IDE の代替バッファ警告ロジック修正

JetBrains IDE での代替バッファ警告ロジックが正しく動作するよう修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26067)

## MCP ping のオプション化とタイムアウト設定

MCP の ping が list コマンドでオプションとなり、設定されたタイムアウトが使用されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26068)

## cloudshell-gca 認証失敗時のエラーメッセージ改善

cloudshell-gca 認証が失敗した場合のエラーメッセージがより分かりやすくなった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26079)

## ContextManager と AgentChatHistory の接続

新しい ContextManager と AgentChatHistory が接続された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25409)

## コマンドラインからのセッション UUID 指定

コマンドライン引数でセッション UUID を手動指定できるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26060)

## 並列タスクトラッカー更新の強制

タスクトラッカーの更新が並列で強制的に実行されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/24477)

## テスト・ドキュメント

- ACP コマンドの復元に関するユニットテストが追加された
- サンドボックスのドキュメントが更新された

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.41.0-nightly.20260428.gc17400b83)

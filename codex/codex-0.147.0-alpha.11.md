## 統合exec出力状態の集約

出力バッファ、通知、クローズド状態、キャンセレーショントークンが`OutputHandles`構造体に統合された。

[参考リンク](https://github.com/openai/codex/pull/37083)

## MCPバインディングのサンプリングステップ間での再利用

サーバー起動がツールカタログリビジョンで安定化した後、公開されたMCPランタイム上に`McpBinding`がキャッシュされるようになった。

[参考リンク](https://github.com/openai/codex/pull/37101)

## APIキーGuardianレビューへのLuna使用

APIキー認証によるGuardian承認レビューに`gpt-5.6-luna`が選択されるようになった。

[参考リンク](https://github.com/openai/codex/pull/37103)

## インタラクティブテレメトリシャットダウンの制限

TUIテレメトリクリーンアップに500msの予算を持つ`OtelProvider::shutdown_with_timeout`が実装された。

[参考リンク](https://github.com/openai/codex/pull/37109)

## セッション単位のコードモード実行制限の追加

`create_session_with_limits`によるセッションスコープのセル実行制限が導入された。

[参考リンク](https://github.com/openai/codex/pull/37114)

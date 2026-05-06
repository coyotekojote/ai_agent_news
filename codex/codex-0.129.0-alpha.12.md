## Git ページネーションフラグのポジション処理

Windows Git の safe-command バイパス脆弱性に対応するセキュリティ修正。Git オプションの安全性マッチングが明示的なリストに分割され、グローバルページネーションフラグ（`--paginate`、`-p`）は unsafe として扱われる一方、パッチ操作（例: `git log -p`）の safe ステータスは維持された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.12)

## MCP Elicitation の Guardian ルーティング

MCP elicitation が Guardian 承認パスを使用する汎用オプトインメカニズムが実装された。Browser Use のオリジンアクセスプロンプトがメタデータに `"codex_request_type": "approval_request"` を設定することで Guardian バリデーションをトリガーできる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.12)

## フォールバックモデルメタデータ警告の重複排除

未解決モデルのフォールバックメタデータ警告がセッション状態で追跡され、セッションごとに 1 回のみ警告されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.12)

## ツールアイテムイベントのライフサイクル発行

app-server のアイテムライフサイクルからツール分析イベントが発行されるようになった。コマンド実行、ファイル変更、MCP コール、動的ツール、コラボレーションツール、Web 検索、画像生成のツールアイテム完了通知が追跡される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.12)

## バグ修正

- TUI Ctrl+C ドラフト永続化が現在の app-event パスを使用して復元された
- OpenTelemetry 診断が明示的に有効化されない限り抑制されるようになった
- 環境コンテキストシェルがハードコードの bash から明示的メタデータに変更された
- コアの MCP リストツールオペレーションが削除された
- ツールハンドラが個別ファイルにリファクタリングされた
- TUI スレッドに明示的な `thread_source = user` メタデータが付与されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.12)

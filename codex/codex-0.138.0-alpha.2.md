## Planモードでの自動アイドルターン制御

Planモードまたは別タスクがアクティブな場合、自動アイドル継続ターンの開始がゲートされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.2)

## スキル拡張へのブリッジ

ホストでロード済みのターンごとスキル結果がスキル拡張に統合され、スキルディスカバリパスと環境ベースのファイル読み取りが保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.2)

## memchrによるバイトスキャン最適化

MCP stdio、Ollamaストリーミング、メッセージ履歴の改行カウントにmemchrが導入され、545倍〜600倍の高速化が実現された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.2)

## SQLiteコンテンション低減

OpenTelemetry SDKのデバッグ/トレースイベントがSQLite永続化前にフィルタリングされ、書き込みボリュームが削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.2)

## プラグインフック読み込みの最適化

フック専用のプラグインロードパスが作成され、不要な機能のスキップにより`hooks/list`のレイテンシが100ms以上改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.2)

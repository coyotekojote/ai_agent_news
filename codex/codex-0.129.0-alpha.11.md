## レスポンス処理 WebSocket リクエストの追加

`response.processed` WebSocket リクエストが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## メッセージ履歴のコア外移動

メッセージ履歴がコアから外部に移動された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## v2 sessionId の Thread への移動

v2 の `sessionId` が `Thread` に移動された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## メモリ用 MCP のスポーン

メモリ用の MCP がスポーンされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## インストール ID 解決のコアスタートアップ外移動

インストール ID の解決がコアのスタートアップから外部に移動された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## コンパクトでのキャッシュキーとサービスティアの伝播

コンパクト処理でキャッシュキーとサービスティアが伝播されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## thread/fork からのセッション ID 返却

`thread/fork` からセッション ID が返却されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## MCP ターンメタデータへのスレッド ID 追加

MCP ターンメタデータにスレッド ID が含まれるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## session_id の追加

`session_id` が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## Codex Apps 認証 elicitation のサポート

Codex Apps の認証 elicitation がサポートされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## 自動バキュームの移動

自動バキュームが移動された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

## バグ修正

- bubblewrap が 0.11.2 に更新された
- TUI で Ctrl+C でスタッシュされたドラフトが `/clear` 後に保持されるよう修正された
- OpenAI ドキュメントサンプルが API キーセットアップと連携するよう調整された
- スレッドの `updated_at` タッチが統合された
- セッションプロトコルで文字列のサービスティアが使用されるようになった
- ビルトイン MCP の Windows パステストが修正された
- テンプレート補間のマルチエージェント使用ヒントサポートがリバートされた
- app-server-client のインプロセステスト状態が分離された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.11)

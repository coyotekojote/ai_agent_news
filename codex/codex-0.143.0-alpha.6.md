## Codex Apps クライアントセットアップの統合

Codex Apps サーバーの分類が統合され、冗長なセットアップ呼び出しが排除された。

[参考リンク](https://github.com/openai/codex/pull/29583)

## サンドボックスの MCP サンドボックス状態消費対応

サンドボックスが codex メタデータから JSON 値を受け入れるようになり、パーミッションプロファイルが必要となり、外部サンドボックス状態が読み取り専用として扱われるようになった。

[参考リンク](https://github.com/openai/codex/pull/29358)

## ブリッジされたログイベントの永続化停止

ブリッジされたログレコードが SQLite シンクでフィルタリングされ、高ボリュームの依存関係イベントがデータベースに到達しなくなった。

[参考リンク](https://github.com/openai/codex/pull/29599)

## Codex Apps 認証 elicitation ハング修正

予約済み Codex Apps サーバー名の存在確認がホスト所有判定の前に必要となり、認証 elicitation テストのハングが防止された。

[参考リンク](https://github.com/openai/codex/pull/29615)

## マルチエージェント v2 ツールの collaboration 名前空間統一

マルチエージェント v2 ツールが固定の「collaboration」名前空間を使用するように標準化され、TOML の設定可能な名前空間オプションが削除された。

[参考リンク](https://github.com/openai/codex/pull/29067)

## `responses` サブコマンドの削除

隠し CLI サブコマンド `codex responses` が削除された。下流の依存がないことを確認した上で廃止された。

[参考リンク](https://github.com/openai/codex/compare/rust-v0.126.0-alpha.3...rust-v0.126.0-alpha.4)

## JWT による AgentIdentity ロード

プログラムエージェントが stdin や環境変数を介して JWT 検証付きの ID トークンを提供できるようになった。

[参考リンク](https://github.com/openai/codex/pull/18904)

## パーミッションプロファイルへの移行

ランタイムの権限モデルが `PermissionProfile` ベースに移行された。レガシー互換ビューはプロファイルから導出されるようになり、承認・サンドボックスの判断もプロファイルを直接参照するように更新された。不要なレガシーポリシーの往復変換も削除された。

[参考リンク](https://github.com/openai/codex/compare/rust-v0.126.0-alpha.3...rust-v0.126.0-alpha.4)

## app-server エラーハンドリングの改善

JSON-RPC のエラーハンドリングがリクエスト境界に集約され、ハンドラーコード全体に散らばっていた処理が統合された。

[参考リンク](https://github.com/openai/codex/pull/19484)

## codex-config への設定ロード統合

設定ロードの責務が `codex-config` クレートに統一された。

[参考リンク](https://github.com/openai/codex/pull/19487)

## `multi_agent_v2` での `max_threads` サポート

`agents.max_threads` 設定が新しい multi_agent_v2 実装でも動作するようになった。

[参考リンク](https://github.com/openai/codex/pull/19733)

## MCP 接続モジュールの分割

モノリシックな MCP マネージャーが個別の責務を持つモジュールに分割された。

[参考リンク](https://github.com/openai/codex/pull/19725)

## バグ修正・改善

- app-server 統合テストのプラグイン起動タスク制御が明示化され、テストでの不要なウォームアップ処理が抑制された
- codex-core の設定テストのタイプパスがクレート移行に合わせて修正された
- Bazel テストのシャード数が 16 に増加され、Windows CI のタイムアウト圧力が軽減された
- 未使用の `ResponseItem::Message.end_turn` フィールドが削除された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.4)

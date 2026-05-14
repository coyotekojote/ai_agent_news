## プラグインマーケットプレイスCLIコマンドの追加

包括的なマーケットプレイス管理コマンドが追加された。`codex plugin add <plugin>@<marketplace>`、`codex plugin list [--marketplace]`、`codex plugin marketplace add/list/upgrade/remove`などの新コマンドが利用可能になった。インストールは設定済みマーケットプレイスに制限され、ローカルスナップショットがパッケージインデックスとして扱われる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## TUIコンポーザーの状態管理リファクタリング

ChatComposerから添付ファイルとポップアップの状態管理が分離された。画像管理、プレースホルダーの再ラベリング、ポップアップライフサイクルが専用の`AttachmentState`と`PopupState`クラスに移動された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## MCP OAuth クライアントIDのサポート

`[mcp_servers.<server>]`配下に明示的な`oauth.client_id`設定が追加された。OAuthプロバイダーが要求する事前登録済みパブリッククライアントIDの指定が可能になった。CLI、app-server、プラグインログイン、MCPスキル依存関係のエントリーポイントに対応。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## ネットワーク承認履歴の表示改善

ネットワーク承認履歴がコマンドではなくターゲットごとに表示されるようになった。以前の不正なエントリ表示が修正され、承認プロトコルとネットワークターゲット（例: `https://example.com:8443`）が表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## Git FSMonitor設定の独立化

Gitメタデータ・ステータスサブプロセスがリポジトリの`core.fsmonitor`設定から独立して動作するようになり、予測可能性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## SIWCユーザー向けモデルリスト優先順位の変更

バンドルリストよりもバックエンドから取得したモデルを優先するようにマージロジックが更新された。制限されたモデルアクセス権限を持つユーザーに対応。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

## バグ修正

サンドボックステストのアイソレーションが改善され、`/tmp/.git`、`/tmp/.agents`、`/tmp/.codex`などのリークしたメタデータマーカーによる後続テストの汚染が防止された。プラグインCLIのコンパイルが修正され、削除された`get_user_layer()`から`get_active_user_layer()`への呼び出しが更新された。リモート環境テストフィクスチャのローカル環境サポート追加や、CLI Codexホームのテストアイソレーションが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.18)

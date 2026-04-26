## ゴール機能の追加

5パートからなる「ゴール」機能が追加された。ゴールの永続化、app-server API、モデルツール、コアランタイム、TUI UX が含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## GPT-5.5 モデルサポート

models.json および関連するコア、app-server、SDK、TUI のフィクスチャが最新のモデルカタログと推論デフォルトに更新され、GPT-5.5 が利用可能なモデルとして追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## プラグインマーケットプレイスの内部リファクタリング

プラグインマーケットプレイスの追加・削除・起動同期の内部処理が codex-core から分離された。キュレートプラグインキャッシュのバージョン管理がショート SHA を使用するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## パーミッションの改善

レガシーの読み取り専用アクセスモードが削除された。互換性ポリシーがプロファイルから導出されるようになり、ランタイム設定がプロファイルベースになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## 設定ロードの改善

設定ロード処理が codex-config に移動され、レガシーの `responses` コマンドが削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## MCP の改善

codex-mcp のアイテムが可視性順に並べ替えられ、未使用の API と重複ヘルパーが整理された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## JWT 認証サポート

JWT ログインおよび環境変数から AgentIdentity をロードする機能が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

## バグ修正

- macOS 署名エンタイトルメントの変更がアルファ版の起動失敗を引き起こしたため元に戻された
- Bedrock GPT-5.4 の推論レベルが修正された
- スレッド再開時のモデルプロバイダーの永続化が復元された
- 承認ポップアップおよびプラグイン MCP ツール検出の不安定なテストが安定化された
- 利用不可のダミーツールがデフォルトで有効化された
- app-server の JSON-RPC エラーハンドリングがリクエスト境界に引き上げられた

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.2)

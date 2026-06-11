## スキルシステムのコアからの分離

スキル拡張機能がコアから分離され、モジュール性が向上した。バックエンドプラグインスキルがエグゼキューター無しで呼び出し可能になった。リモートスキルリソースツールが公開された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## MCPサーバー登録のカタログベース解決

MCPサーバー登録がカタログを通じて解決されるようになり、サーバー検出メカニズムが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## リモートコンパクションv2のデフォルト有効化

リモートコンパクションv2がデフォルトで有効になり、コンテキスト管理のパフォーマンスが向上した。comp_hashの変更時にコンパクトが実行されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## コンテキスト残量ツールの追加

コンテキストの残量を確認できるツールが追加され、セッション中のコンテキスト使用状況の可視化が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## PATワークスペース制限の強制

PATのワークスペース制限が強制されるようになり、認証セキュリティが強化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## ユーザー指示のインジェクテッドプロバイダー経由読み込み

ユーザー指示がインジェクテッドプロバイダーを通じて読み込まれるようにリファクタリングされ、指示処理の柔軟性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## Responses APIメタデータの統合

Responses APIのCodexメタデータが統合され、APIレスポンスの処理が効率化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## ARM64 MinGW互換性サポート

ARM64 MinGWのpowl互換性サポートが提供され、クロスプラットフォーム対応が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## 致命的終了時のTUIセッション情報表示

致命的エラーで終了する際にTUIセッション情報が表示されるようになり、デバッグが容易になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## 画像リサイズ時のメタデータ保持

プロンプト画像のリサイズ時にメタデータが保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

## レガシーWindowsサンドボックス依存の削除

TUIのレガシーWindowsサンドボックス依存が削除され、コードが整理された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.11)

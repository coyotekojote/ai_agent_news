## TUI 推論制御のクイック操作

TUI に推論レベルのクイック制御が追加された。Alt+, で推論レベルを下げ、Alt+. で上げることができる。また、モデルアップグレードを承認した際に、推論設定が古い値を引き継がず新しいモデルのデフォルトにリセットされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## Amazon Bedrock のファーストクラスサポート

OpenAI 互換プロバイダー向けに Amazon Bedrock のファーストクラスサポートが追加された。AWS SigV4 署名および AWS クレデンシャルベースの認証に対応している。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## Hooks の安定化

Hooks が安定版となり、config.toml 内でインライン設定および managed requirements.toml での管理が可能になった。MCP ツール、apply_patch、長時間実行の Bash セッションの監視にも対応した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## リモートプラグインマーケットプレイスの改善

リモートプラグインマーケットプレイスの一覧表示と直接読み取りが可能になった。詳細検索の信頼性が向上し、結果ページのサイズも拡大された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## セキュリティ依存関係の修正

高深刻度の依存関係アラートに対応し、パッチ済みの JS および Rust 依存関係がピン留めされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## ビルド改善

Rust 開発ビルドのデバッグ情報オーバーヘッドが削減された。バックトレースの有用性は維持されている。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

## Python SDK 型定義の更新

生成された Python app-server SDK の型定義が最新のスキーマに基づいてリフレッシュされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.1)

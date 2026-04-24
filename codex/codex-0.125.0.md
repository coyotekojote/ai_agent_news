## App-server Unix ソケットトランスポート

App-server が Unix ソケットトランスポートに対応し、ページネーション対応の resume/fork 操作、スティッキー環境、リモートスレッド設定/ストアの配管がサポートされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## リモートプラグインのインストールとマーケットプレイスアップグレード

リモートプラグインのインストールおよび設定済みマーケットプレイスのアップグレードが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## パーミッションプロファイルの永続化

パーミッションプロファイルが TUI セッション、ユーザーターン、MCP サンドボックス状態、シェルエスカレーション、app-server API をまたいで永続化（ラウンドトリップ）されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## モデルプロバイダーディスカバリー

モデルプロバイダーがモデルディスカバリーを所有するようになり、AWS/Bedrock のアカウント状態がアプリクライアントに公開されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## `codex exec --json` の推論トークンレポート

`codex exec --json` が推論トークンの使用量メトリクスを報告するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## ロールアウトトレーシングの拡張

ロールアウトトレースがツール、コードモード、セッション、マルチエージェントの関係を記録するよう拡張され、デバッグリデューサーコマンドも追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

## バグ修正

- `/review` の中断が TUI をハング/ウェッジさせる問題を修正
- exec-server がプロセス終了後にストリームクローズを適切に待機するようになり、バッファされたコンテンツがドロップされなくなった
- プロジェクト設定の信頼処理で明示的な untrusted 設定が正しく尊重されるよう修正
- Windows サンドボックス起動時の複数 CLI バージョンおよびアプリディレクトリの処理が改善された
- 通知バースト中の WebSocket クライアントの切断が軽減された
- MultiAgentV2 のスレッド制限と画像 MIME タイプの設定バリデーションが強化された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.125.0)

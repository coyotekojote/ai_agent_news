## ゴールランタイムのエクステンション移行完了

ゴールランタイムのエクステンションへの移行が完了し、コア動作との整合性が確保された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## v2エージェントのリロード

v2エージェントがデリバリー時にリロードされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## リモートコントロールのペアリングステータス

リモートコントロール機能にペアリングステータスのトランスポートとRPC公開が追加された。無効状態でもペアリングが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## TUI起動の高速化

プラグインディスカバリーの再利用によりTUI起動が高速化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## resume --lastの最適化

`resume --last`でステートDBが最初に使用されるようになり、セッション復旧が最適化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## マルチエージェントv2メッセージの暗号化

マルチエージェントv2のメッセージペイロードが暗号化されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## Linuxサンドボックスの改善

プロキシ経由のLinuxサンドボックスでsocketpairが許可されるようになった。長いプロキシソケットパスの問題が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## バグ修正

ストリーミング出力時の空白行の重複が修正された。キャンセルされたプロンプトのカーソル位置が修正された。`/goal`コマンドの使用方法ドキュメントが修正された。Windowsワークスペースのディープリンク経由での起動がサポートされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

## インフラストラクチャの改善

bashシェルのフォールバックオプションが追加された。ランタイムワークスペースルートがAPIで絶対パスになった。環境シェル情報のトラッキングが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.5)

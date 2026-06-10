## MCP接続マネージャーAPIの整理

MCP接続マネージャーのAPI可視性と順序が整理された。接続管理の内部構造が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## Streamable HTTP初期化リトライ

Streamable HTTPの初期化失敗時にリトライが行われるようになった。接続の安定性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## Pythonゴール操作の追加

Pythonゴールルーティングの基盤が追加され、プライベートPythonゴール操作が実装された。ゴールワークフローにおけるPythonサポートが拡張された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## 非TTY環境でのCtrl-Cハンドリング

非TTYの統合実行環境でCtrl-Cが適切に処理されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## MCP OAuth認証情報の改善

使用不可なMCP OAuth認証情報がログアウト状態として報告されるようになり、ユーザーへの通知が明確になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## ホスト型Apps MCPのルーティング変更

ホスト型Apps MCPがextensionsを通じてルーティングされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## TUIレガシー依存関係の削減

TUIコアのレガシー依存関係が削減され、コードベースのモダナイゼーションが進められた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## ゴール完了後の新規ゴール作成

ゴール完了後に新しいゴールを作成できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

## プラグインリモートアンインストールの修正

リモートアンインストールでプラグインサービスルートが正しく使用されるよう修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.2)

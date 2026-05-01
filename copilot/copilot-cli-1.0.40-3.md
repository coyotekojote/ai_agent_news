## MCP サーバーの client_credentials OAuth 対応

MCP サーバーで `client_credentials` OAuth グラントタイプがサポートされ、ブラウザなしの完全ヘッドレス認証が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

## /research コマンドのオーケストレーター/サブエージェントモデル対応

`/research` コマンドがオーケストレーター/サブエージェントモデルを使用するようになり、より徹底的で信頼性の高いディープリサーチ結果が得られるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

## オートパイロットの継続メッセージ制限

オートパイロットモードで継続メッセージがデフォルト 5 回に制限されるようになった。`--max-autopilot-continues` で設定可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

## 自動アップデート時の旧バージョンクリーンアップ

自動アップデート時に古い CLI パッケージバージョンが自動的にクリーンアップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

## リモートセッションのステータスライン改善

リモートセッションのステータスラインにローカルコンテキストではなく、リモートの作業ディレクトリとブランチが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

## バグ修正

- サブエージェントが親セッションの設定を継承するのではなく、自身のモデルのツール検索サポートを正しく評価するようになった
- `/new` および `/resume` コマンドで保留中のメッセージが新しいセッションに引き継がれなくなった
- 大きなファイル添付送信時に CPU が 100% でハングする問題が修正された
- Mission Control バックドセッションのセッション再開ピッカーで重複エントリが排除された
- セッション再開セレクターでサマリーが 1 行に表示され、カラム幅に切り詰められるようになった
- Ctrl+C 時に「Exiting…」メッセージが即座に stderr に出力されるようになった

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.40-3)

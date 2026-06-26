## autoMode.classifyAllShell設定の追加

すべてのBash/PowerShellコマンドを任意コード実行パターンだけでなくautoモード分類器を通してルーティングする`autoMode.classifyAllShell`設定が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## autoモード拒否理由の表示

autoモードの拒否理由がトランスクリプト、拒否トースト、`/permissions`の最近の拒否に表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OpenTelemetryアシスタントレスポンスログの追加

モデルのレスポンステキストを含む`claude_code.assistant_response` OpenTelemetryログイベントが追加された。`OTEL_LOG_ASSISTANT_RESPONSES=1`が設定されていない限りデフォルトで秘匿される。未設定の場合は`OTEL_LOG_USER_PROMPTS`に従う。

[参考リンク](https://code.claude.com/docs/en/changelog)

## bashモードのファイルパスオートコンプリート

bashモード（`!`）にライブファイルパスオートコンプリートが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP認証の起動通知

MCPサーバーが認証を必要とする場合に起動時通知が表示され、`/mcp`を案内するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アイドルバックグラウンドシェルコマンドの自動メモリ解放

メモリ負荷時にアイドル状態のバックグラウンドシェルコマンドが自動的に解放されるようになった。`CLAUDE_CODE_DISABLE_BG_SHELL_PRESSURE_REAP=1`で無効化可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /modelのステール状態修正

`/login`直後に`/model`およびその他のクライアントデータゲートUIが古い/空の状態を表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンド化時の誤キャンセル修正

すべての実行中タスクが新しいセッションに引き継がれる場合に、バックグラウンド化（←←）が「N background tasks would be abandoned」で誤ってキャンセルされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ピン留めバックグラウンドエージェントの再プロンプト修正

ピン留めされたバックグラウンドエージェントが自動アップデート後に毎回「Continue from where you left off」と再プロンプトされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンド化時のファントムサブエージェント修正

メインターンをバックグラウンド化した際にメイン会話を再実行するファントム「general-purpose (resumed)」サブエージェントが生成される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントパネルの兄弟エージェント非表示修正

サブエージェントを表示中にエージェントパネルが兄弟エージェントを隠す問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェント起動結果の改善

バックグラウンドエージェントの起動結果がClaudeに「レスポンスを終了する」よう指示しなくなり、エージェント実行中に他のタスクへの作業を継続するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP headersHelper認証の自動再接続

MCP `headersHelper`認証でツールコールが401/403を返した際にヘルパーが自動的に再実行され再接続されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグイン自動リネーム

マーケットプレイスの`renames`マップが自動的に適用され、設定が新しい名前に更新されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /add-dirメッセージの改善

ディレクトリが既にワーキングディレクトリである場合の`/add-dir`メッセージが改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

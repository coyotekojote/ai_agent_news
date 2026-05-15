## 実験的MCPサーチコマンドの追加

実験的な`/mcp search`コマンドが追加され、レジストリからMCPサーバーの検索とインストールが可能になった。MCPおよび外部ツールの遅延ロード機能を備えたツール検索も追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

## 推論エフォートピッカーに「None」オプション追加

推論エフォートピッカーに「None」オプションが追加され、モデルの推論を無効化できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

## COPILOT_PLUGIN_DIR_ONLY環境変数の追加

`COPILOT_PLUGIN_DIR_ONLY`環境変数が追加され、自動プラグイン検出を無効化して`--plugin-dir`使用時に決定論的なプラグイン構成が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

## メモリ権限プロンプトのスコープ表示

メモリ権限プロンプトがアクセスのスコープを明確に表示するようになり、タイムラインエントリに「(for user)」や「(shared with repository collaborators)」が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

## PowerShell 5.x互換性の改善

レガシーPowerShell 5.x環境で`&&`チェーンの使用が回避され、構文エラーが削減された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

## バグ修正

スクロールビューからのテキストコピーでソフトラップされた行に余分な改行やインデントが追加されなくなった。入力フィールドのカーソル位置がワイド文字（CJK、絵文字）で正しく処理されるようになった。フック関数（preToolUse、postToolUse、subagentStart、subagentStop）がサブエージェントのツールコールで正しく実行されるようになった。`--plugin-dir`経由でロードされたプラグインがエージェントをタスクサブエージェントとして正しく登録するようになった。リポジトリコンテキストがない場合にメモリストレージが利用可能なスコープを適切に制限するようになった。`--plugin-dir`と`--additional-mcp-config`が`--server`/`--headless`モードで動作するようになった。コンテンツフィルタリングされたレスポンスが空白のターンではなく説明を表示するようになった。PromptFrame UIがtmux内でghostty、WezTerm、kittyターミナルで正しくレンダリングされるようになった。MCP OAuthトークンの検索がアクティブセッションに正しくスコープされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.49-0)

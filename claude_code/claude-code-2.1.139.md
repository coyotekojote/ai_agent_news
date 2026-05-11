## Agent View（リサーチプレビュー）

Claude Codeの全セッション（実行中・ユーザー待ち・完了）を一覧表示する新しいビューが追加された。`claude agents` コマンドで起動できる。

[参考リンク](https://code.claude.com/docs/en/agent-view)

## `/goal` コマンドの追加

完了条件を設定すると、Claudeがその条件を満たすまで複数ターンにわたって自律的に作業を続ける機能が追加された。インタラクティブモード、`-p` モード、Remote Controlで動作し、経過時間・ターン数・トークン数がオーバーレイパネルでリアルタイム表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/scroll-speed` コマンドの追加

マウスホイールのスクロール速度をライブプレビュー付きで調整できるコマンドが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude plugin details` コマンドの追加

`claude plugin details <name>` でプラグインのコンポーネント一覧とセッションごとの推定トークンコストを表示できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## トランスクリプトビューのナビゲーション強化

`?` でキーボードショートカット一覧、`{`/`}` でユーザープロンプト間のジャンプ、`v` でショートカットパネルの切り替えが可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フックの `args: string[]` フィールド（exec形式）

コマンドをシェルを介さず直接実行するexec形式が追加され、パスプレースホルダのクォートが不要になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フックの `continueOnBlock` オプション

`PostToolUse` フックに `continueOnBlock` 設定オプションが追加された。`true` に設定するとフックの拒否理由をClaudeにフィードバックしてターンを継続できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP stdioサーバーへの `CLAUDE_PROJECT_DIR` 環境変数の提供

MCP stdioサーバーがフックと同様に `CLAUDE_PROJECT_DIR` 環境変数を受け取るようになった。プラグイン設定のコマンドで `${CLAUDE_PROJECT_DIR}` を参照可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートMCPサーバーの再接続リトライ

一時的な障害時のリモートMCPサーバー再接続リトライが全ユーザーに対して有効化された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントAPIリクエストヘッダーの追加

`x-claude-code-agent-id` / `x-claude-code-parent-agent-id` ヘッダーが追加され、`claude_code.llm_request` OTELスパンに `agent_id` / `parent_agent_id` 属性が含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## APIキー設定時の機能制限

`ANTHROPIC_API_KEY` / `apiKeyHelper` / `ANTHROPIC_AUTH_TOKEN` が設定されている場合、Claude.aiログインが存在してもRemote Control・スケジュール・MCPコネクタ・通知設定が無効化されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## VS Code: 閉じたセッションタブの再開ショートカット

VS CodeでCmd/Ctrl+Shift+Tを押すと直近に閉じたセッションタブを再開できるようになった。`claudeCode.enableReopenClosedSessionShortcut` で設定可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 改善

コンパクション時にモデルがユーザーの機密指示を保持するようプロンプトが改善された。`/mcp` の再接続がリスタート不要で `.mcp.json` の編集を反映するようになり、失敗時にHTTPステータスとURLが表示されるようになった。`/context all` のスキルごとのトークン推定がモデルのトークナイザーを考慮し丸め値で表示されるようになった。`claude plugin install` がマーケットプレイスの自動リフレッシュとリトライを行うようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

期限切れの認証情報と `forceRemoteSettingsRefresh` ポリシー設定が `claude auth` コマンドをブロックするデッドロックが修正された。`autoAllowBashIfSandboxed` が `$VAR` や `$(cmd)` などのシェル展開を含むコマンドを自動承認しない問題が修正された。フックがターミナルに書き込むとインタラクティブプロンプトが壊れる問題が修正された。HTTP/SSE MCPサーバーからの非プロトコルデータストリーミングによるメモリ無限増加が修正された（SSEフレームあたり16MBに制限）。その他多数のUI・スクロール・プラグイン関連のバグが修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.139)

## バックグラウンドセッション設定フラグの追加

`claude agents`に新しいフラグが追加され、ディスパッチされたバックグラウンドセッションの構成が可能になった。`--add-dir`、`--settings`、`--mcp-config`、`--plugin-dir`、`--permission-mode`、`--model`、`--effort`、`--dangerously-skip-permissions`が利用可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ルートレベルSKILL.mdによるスキル公開

ルートレベルに`SKILL.md`があり`skills/`サブディレクトリがないプラグインが、スキルとして自動的に公開されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグイン詳細でのLSPサーバー表示

`/plugin`の詳細ペインと`claude plugin details`で、プラグインが提供するLSPサーバーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /web-setupの既存接続警告

`/web-setup`が既存のGitHub App接続を置き換える前に警告を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fastモードのデフォルトモデル変更

FastモードがデフォルトでOpus 4.7を使用するようになった（以前はOpus 4.6）。`CLAUDE_CODE_OPUS_4_6_FAST_MODE_OVERRIDE=1`を設定することでOpus 4.6に固定可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リアクティブコンパクションの改善

リアクティブコンパクションが改善され、最初の要約試行が元のリクエストのオーバーフローサイズからシードされるようになり、フルコンテキストに近い無駄なリトライが回避されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フック設定エラーメッセージの改善

`SessionStart`/`Setup`/`SubagentStart`にプロンプトまたはエージェントタイプのフックを設定した場合、「代わりにcommandタイプのフックを使用してください」という明確なエラーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

`MCP_TOOL_TIMEOUT`がリモートHTTPおよびSSE MCPサーバーのリクエスト単位のフェッチタイムアウトを引き上げない問題が修正され、ツールコールが60秒で上限に達する問題が解消された。バックグラウンドセッションが既存のgitワークツリーを認識せず、`EnterWorktree`が重複作成を拒否して`Edit`がブロックされる問題が修正された。macOSのスリープ/ウェイク後にバックグラウンドセッションが消失しデーモン再接続が失敗する問題が修正された。バイナリアップグレード後（例：`brew upgrade`）にデーモンがクリーンに終了しない問題が修正された。Chrome拡張が共有タブなしで接続された際にバックグラウンドエージェントがクラッシュループする問題が修正された。アタッチされた`claude agents`セッションでリンクのクリックが修正された。`claude agents`の「v to open in editor」が`$EDITOR`/`$VISUAL`ではなくデーモンのデフォルトエディタを使用する問題が修正された。Windowsでネットワークドライブの作業ディレクトリ使用時に`claude agents`がデッドロックする問題が修正された。Apple Terminalなどの256色限定ターミナルでの背景色のにじみが修正された。`claude --bg --dangerously-skip-permissions`がリタイア/ウェイク間で永続化されない問題が修正された。最初のメッセージがリンクの場合にセッションタイトルがURLから導出される問題が修正された。リモートクライアントからの冗長な`set_model`リクエストが重複した`/model`パンくずを挿入する問題が修正された。`skills: ["./"]`を使用するプラグインで誤った「パスがプラグインディレクトリを超えている」エラーが表示される問題が修正された。プラグインキャッシュのクリーンアップがアクティブなプラグインバージョンディレクトリを削除する問題が修正された。`/plugin`ブラウズペインで新しく公開されたプラグインに「0 installs」と表示される問題が修正された。プラグインアドバイザリがデフォルトフォルダを上書きする`plugin.json`キーをすべて名前で表示しない問題が修正された。Usage Policyの拒否メッセージから古い`/model claude-sonnet-4-20250514`のサジェストが削除された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.142)

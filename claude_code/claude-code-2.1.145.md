## claude agents --jsonコマンドの追加

`claude agents --json`が追加され、ライブClaude セッションをJSON形式でリスト表示できるようになった。tmux-resurrect、ステータスバー、セッションピッカーなどのスクリプティングに利用可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OTELスパンへのエージェントID属性追加

`claude_code.tool` OTELスパンに`agent_id`と`parent_agent_id`属性が追加され、バックグラウンドサブエージェントスパンがディスパッチ元のAgentツールスパンの下にネストされるようトレースの親子関係が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ステータスラインJSONにGitHubリポジトリ・PR情報追加

ステータスラインのJSON入力に、検出された場合にGitHubリポジトリおよびPR情報が含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /pluginのディスカバー・ブラウズ画面でプラグイン詳細表示

`/plugin`のディスカバーおよびブラウズ画面で、インストール前にプラグインのコマンド、エージェント、スキル、フック、MCP/LSPサーバーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsタブタイトルに入力待ちカウント表示

`claude agents`のターミナルタブタイトルに入力待ちカウントが表示されるようになり、Alt-Tabしたウィンドウでエージェントがアテンションを必要としているタイミングがわかるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スラッシュコマンド・@メンション候補のマウス操作対応

スラッシュコマンドと@メンションの候補リストがフルスクリーンモードでマウスホバーとクリックをサポートするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## StopおよびSubagentStopフック入力の拡張

StopおよびSubagentStopフックの入力に`background_tasks`と`session_crons`フィールドが含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Readツールのトークン制限時の改善

Readツールがファイル全体読み取りがトークン制限を超えた場合にハードエラーの代わりに、切り詰められた最初のページを「PARTIAL view」通知付きで返すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

Bashコマンド内の許可リスト外環境変数への素の変数代入が自動承認される権限プロンプトバイパスが修正された。MCPプロンプトスラッシュコマンドが必須引数省略時にサーバーの生のバリデーションエラーを表示する問題が修正され、欠落引数名と期待される使用法が表示されるようになった。ターミナルのリサイズやリフォーカス後にスピナーと経過時間表示がキー入力まで停止する問題が修正された。クロスプロジェクト再開ヒントがデフォルトのWindows PowerShell 5.1で失敗する問題が修正され、Windowsではコマンドセパレータに`;`を使用するようになった。エージェントビューのリプライペインで音声プッシュトゥトークが機能しない問題が修正された。複数タスクが同時作成された場合にタスクリストがランダム順序でレンダリングされる問題が修正された。マーケットプレイスが既にインストール済みの場合に古い「Failed to install Anthropic marketplace」バナーが表示される問題が修正された。`gh pr create`やその他のPR状態変更コマンド実行後にフッターのPRバッジが即座に更新されない問題が修正された。非ASCII名のAgent Teamsチームメイトが無効なヘッダーエンコーディングによりすべてのAPI呼び出しで失敗する問題が修正された。`/review`がClassic Projectsを持つリポジトリでエラーになる非推奨の`projectCards` GraphQLクエリを使用する問題が修正された。`claude plugin validate`が`skills:`エントリがディレクトリではなくファイルを指している場合にフラグを立てない問題が修正され、親ディレクトリを提案するようになった。`context: fork`を使用するスキルが実行ではなく自身を繰り返し再呼び出しする無限ループが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

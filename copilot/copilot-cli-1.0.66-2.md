## 異なるプラグインからの同名スキルの共存

異なるプラグインからの同じ名前のスキルが共存できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## インテグレーションによるCLIユーザー設定の読み書き

インテグレーションがCLIユーザー設定の読み取りと書き込みを行えるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## LSPサーバーログの表示

`/lsp logs`およびread_agentでLSPサーバーログが表示可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## gh CLIが未インストール時のインストールプロンプト

GitHubリポジトリでgh CLIが未インストールの場合にインストールを促すプロンプトが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## GitHubアタッチメントバリアントのプロンプトレンダリング対応

プロンプトレンダリングにGitHubアタッチメントバリアントが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## トークナイザーの並列バックグラウンド初期化

トークナイザーの起動がバックグラウンドスレッドで並列に行われるようになり、パフォーマンスが向上した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## タイムラインにプロンプト送信時刻を表示

タイムラインのユーザープロンプト横に送信時刻が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## /share機能のセッション表示管理改善

`/share`機能のセッション表示管理が改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## AGENTS.md/CLAUDE.md/Copilot指示ファイルの@スタイルインポート拡張

AGENTS.md、CLAUDE.md、Copilot指示ファイルにおける@スタイルインポートが拡張された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## /pr autoのCI・レビュー・マージキュー対応拡張

`/pr auto`機能がCI、レビュー、マージキューの各ステージを通じて拡張された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## コンパクトタイムラインのコンテンツ表示改善

コンパクトタイムラインのコンテンツ表示メカニズムが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## 拡張モードトグルの設定保持修正

拡張モードのトグルが選択された設定を正しく保持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## アタッチされたシェルコマンドキャンセル後のプロンプトフォーカス復元

アタッチされたシェルコマンドをキャンセルした後にプロンプトのフォーカスが正しく復元されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## バックグラウンドgit操作の並行コマンド干渉防止

バックグラウンドのgit操作が並行して実行されるコマンドと干渉しないようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## セッション履歴の破損からの復旧

読み込み時に破損したセッション履歴から正しく復旧するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## /afterおよび/everyのスケジュールプロンプトの改行保持

`/after`および`/every`を使用したスケジュールプロンプトで改行が正しく保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## /worktreeタスクの複数行タスク整合性保持

`/worktree`タスク開始時に複数行タスクの整合性が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## /cdパス補完のキー操作同期

`/cd`パス補完でEnter、Escape、Tabの動作が同期されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## セッションストアの検索・コンテキスト検索の応答性維持

セッションストアの検索とコンテキスト検索の応答性が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## macOSデスクトップ通知のCLI対応

CLIからmacOSデスクトップ通知が正しく機能するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## WSLでのWindows環境変数未使用時の画像ペースト修正

Windows環境変数が利用できない場合のWSLでの画像ペーストが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## 隣接タスク削除時のタスク選択保持

隣接するタスクを削除した際にタスク選択が正しく保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## read_agentのsince_turn: 0修正

`read_agent`の`since_turn: 0`がターン0を正しく含むように修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

## MCP初期化時の非JSON出力フィルタリング

MCPサーバー初期化時の非JSON出力が正しくフィルタリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.66-2)

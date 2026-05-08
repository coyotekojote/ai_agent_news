## OTEL 向けフィードバックサーベイの有効化

`CLAUDE_CODE_ENABLE_FEEDBACK_SURVEY_FOR_OTEL` が追加され、OpenTelemetry 経由でレスポンスを取得している企業向けにセッション品質サーベイを再有効化できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## オートモードの hard_deny ルール

`settings.autoMode.hard_deny` が追加され、ユーザーの意図や許可例外に関わらず無条件でブロックするオートモード分類ルールを設定できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## WSL2 での画像ペースト対応

WSL2 で xclip/wl-paste が画像データを読み取れない場合に PowerShell フォールバックを使用して Windows クリップボードからの画像ペーストが動作するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## スラッシュコマンドダイアログの視覚的一貫性改善

スラッシュコマンドダイアログ全体でフッターヒント、ダイアログ間隔、矢印キースタイリングが標準化された。ダイアログフレームがローディング中にポップインするのではなく即座に表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ワークツリー衝突時のエラーメッセージ改善

`--worktree` が既存または古いワークツリーと衝突した際のエラーメッセージが改善された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## プラグインマーケットプレイスの削除キー変更

プラグインマーケットプレイスの削除キーが `r`（リトライと競合）から `d`（他の削除操作と統一）に変更された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## MCP サーバーの /clear 後消失修正

`.mcp.json`、プラグイン、および claude.ai コネクタで設定された MCP サーバーが VS Code 拡張、JetBrains プラグイン、Agent SDK で `/clear` 後にサイレントに消失する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ログインループの修正

並行するクレデンシャル書き込みが新しくローテーションされた OAuth トークンを上書きし、再ログインを強制するまれなログインループが修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## MCP OAuth リフレッシュトークンの修正

複数のサーバーが同時にリフレッシュする際に MCP OAuth リフレッシュトークンが失われる問題が修正された。複数のリモート MCP サーバーを持つユーザーは毎日の再認証が不要になった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## 拡張思考のリダクションブロック修正

ツールコール後に拡張思考がリダクションされた思考ブロックを出力した際の API エラー（400）が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## アンダースコアを含むパスでのセッション再開修正

プロジェクトパスにアンダースコアが含まれる場合に `--resume` / `--continue` がセッションを見つけられない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## プランモードのファイル書き込みブロック修正

一致する `Edit(...)` 許可ルールが存在する場合にプランモードがファイル書き込みをブロックしない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## プラグインフックのキャッシュクリーンアップ修正

キャッシュクリーンアップが実行中のセッションで使用中のバージョンを削除した際にプラグインの `Stop`/`UserPromptSubmit` フックが失敗する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## bash 出力とコードブロックの色表示修正

bash コマンド出力およびマークダウンコードブロックで色が誤った位置に表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ReasonML 差分の表示修正

ReasonML の差分が word-diff の境界で壊れた「undefined」テキストアーティファクトを表示する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ワークツリー終了ダイアログの修正

ワークツリー削除後にワークツリー終了ダイアログが誤ったディレクトリの未コミットファイルについて警告する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## @ ファイルピッカーの修正

セッション中に作成されたファイルが小規模な非 git ディレクトリで `@` ファイルピッカーにマッチしない問題が修正された。また、100 エントリ以上のディレクトリで `@` メンションファイルピッカーがファイルを見つけられない問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## 失敗したツールコールの表示修正

フルスクリーンモードで出力が切り捨てられた際に失敗したツールコールがクリックで展開できない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## Backspace と Ctrl+Backspace の入れ替わり修正

拡張キーモードが永続するターミナルで Ctrl+G を使用して外部エディタを開いた後に Backspace と Ctrl+Backspace が入れ替わる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /usage の週次リセット表示修正

`/usage` の週次リセットがカレンダー日付ではなく時刻を表示する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## CJK ターミナルでのウェルカムバナー修正

ウェルカムバナーの省略記号が CJK ターミナルでカラムオーバーフローを引き起こす問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /insights のクラッシュ修正

セッション履歴に不正な入力フィールドを持つツールコールが含まれる場合に `/insights` がクラッシュする問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## レンダラーのクラッシュ修正

ツールの折りたたみ分類がセッション中に変更された際のレンダラークラッシュが修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## plugin.json のスキル設定修正

`plugin.json` の `skills` エントリがプラグインのデフォルト `skills/` ディレクトリを隠す問題が修正された。ファイルパスの一覧表示がサイレントに失敗する代わりにエラーを表示するようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## IDE シェル統合ロックファイルの修正

IDE シェル統合ロックファイルが `CLAUDE_CONFIG_DIR` を尊重しない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ストリーミング中のコピー修正

ストリーミング中にコピーしたターミナル出力に末尾の空白が含まれる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## プラグインのアンインストール・有効/無効の修正

プラグインのアンインストールおよび有効/無効がスラッグの大文字小文字を区別してマッチしていた問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ツールエラー切り捨てマーカーの修正

サロゲートペア文字列でツールエラー切り捨てマーカーが負の数を表示する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## SessionStart フック環境変数の修正

`CLAUDE_ENV_FILE` SessionStart フックからの環境変数が `/resume` や `/clear` 後に古くなる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /branch のセッションタイトル修正

ペーストされた複数行の名前が指定された場合に `/branch` が複数行のセッションタイトルを保存する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## テキスト折り返しの修正

カラム境界で折り返されたテキストの 2 行目に不要な先頭スペースが表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ダイアログの Esc 修正

`/install-github-app`、`/desktop`、`/resume`、`/web-setup` で Esc がダイアログを閉じない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /doctor の MCP スキーマエラー修正

`/doctor` の MCP スキーマエラーが不足しているフィールド名やソースファイルパスを表示しない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## Bash パーミッションプロンプトの修正

Bash パーミッションプロンプトがユーザー可読な説明の代わりに内部パーサー診断を表示する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## スペースを含むプラグインスラッシュコマンドの修正

スペースを含むプラグインスラッシュコマンド（例：`/myplugin review`）がネームスペース形式に解決されない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## AskUserQuestion の複数選択修正

`AskUserQuestion` が配列として提供された複数選択の回答を破棄する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /clear のセッションラベル修正

`/clear <name>` がクリアされたセッションを `/resume` 用にラベル付けしない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## CronList 出力の修正

`CronList` 出力に修飾子とスケジュールされたプロンプトが欠落する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## フルスクリーンモードの CJK 文字修正

フルスクリーンモードで「Jump to bottom」オーバーレイが CJK 文字に色のアーティファクトを残す問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## マークダウンテーブルのレンダリング修正

ストリーミング中に幅広のマークダウンテーブルがターミナルスクロールバックに古い枠線付きレンダーを残す問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## ペーストテキストの切り捨て修正

ペーストテキストプレースホルダーを含む長いプロンプトが自動切り捨てされた際にペーストされたテキストがサイレントにドロップされる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /release-notes の更新修正

チェンジログのリフレッシュに失敗した後に `/release-notes` が古いバージョンのまま動かなくなる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /mcp サーバーリストのスクロール修正

ターミナルに収まるサーバー数を超えた場合に `/mcp` サーバーリストがスクロールしない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## 入力途中のスラッシュコマンド自動補完修正

最初のスラッシュコマンド後に入力途中のスラッシュコマンド自動補完が動作しない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## オートスクロールの修正

`autoScrollEnabled: false` の状態で下部にスクロールするとオートフォローが再度有効になる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## プロンプト候補の自動送信修正

空の入力で Enter を押すとプロンプト候補が Tab や矢印キーでの選択を待たずに自動送信される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## キーボードショートカットヒントの修正

キーボードショートカットヒントが `keybindings.json` でリバインドされたキーを反映しない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /settings の言語変更修正

`/settings` での言語変更が確認後に Escape で元に戻される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## /terminal-setup の自動補完修正

`/terminal-setup` が部分的なプレフィックスではなく完全一致でのみ自動補完に表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## AskUserQuestion ダイアログの修正

`AskUserQuestion` ダイアログで「Chat about this」を選択すると質問テキストが消去される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## MCP ツール結果の表示修正

サーバーがコンテンツブロックを返した際に MCP ツール結果が非表示になる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.136)

## `/config key=value` 構文の追加

`/config key=value` 構文でプロンプトから直接設定を変更できるようになった（例: `/config thinking=false`）。インタラクティブモード、`-p` モード、Remote Controlで利用可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `sandbox.allowAppleEvents` オプトイン設定の追加

macOSでサンドボックス化されたコマンドがApple Eventsを送信できるようにする `sandbox.allowAppleEvents` 設定が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `CLAUDE_CLIENT_PRESENCE_FILE` 環境変数の追加

マーカーファイルを指定する `CLAUDE_CLIENT_PRESENCE_FILE` 環境変数が追加され、ユーザーがPC前にいる間はモバイルプッシュ通知を抑制できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バンドルBunランタイムを1.4にアップグレード

バンドルされているBunランタイムがバージョン1.4にアップグレードされた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長い段落のストリーミング改善

長い段落のテキストが最初の改行を待たずに行単位で表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 自動リトライの改善

思考中のAPI接続切断がエラー表示ではなく自動的にリトライされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントパネルの改善

アイドル状態のサブエージェントが30秒後に自動非表示になり、リストが5行に制限されスクロールヒントが表示されるようになった。キーボードヒントもフッターに表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP OAuthブラウザページの改善

MCP OAuthブラウザページがClaude Codeのビジュアルスタイルに統一され、成功時に自動クローズされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンモードのURL開封動作変更

フルスクリーンモードでのURL開封にCmd+クリック（macOS）/ Ctrl+クリックが必要になり、ネイティブターミナルの動作に統一された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## メモリ改善行の表示簡略化

`Improved N memories` 行がverboseモード以外では個別ファイルをリスト表示しなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプトキャッシュの修正

カスタム `ANTHROPIC_BASE_URL` およびFoundryで、リクエストごとに変わるアテステーショントークンによりプロンプトキャッシュの読み取りが機能しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネットワークドライブでのWrite/Edit修正

ネットワークドライブやクラウド同期フォルダでWrite/Editが0バイトまたは切り詰められたファイルを生成する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## macOSでのopen/osascript/ブラウザ認証の修正

Apple Eventsエンタイトルメントの追加により、macOSで `open`、`osascript`、ブラウザベースの認証フローがエラー -600 で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 起動時のリグレッション修正

2.1.169で導入された起動リグレッション（新規環境で1回の起動につき約120ms遅延）が修正され、MCPサーバー未設定時に管理設定フェッチを待たなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネットワーク劣化時の起動ブロッキング修正

ネットワーク劣化時にアカウント設定フェッチが遅い場合、起動時にターミナルが最大15秒間ブランクでブロックされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `.claude.json` 破損時の起動クラッシュ修正

`.claude.json` にnullのプロジェクトエントリが含まれている場合の起動クラッシュ（`TypeError: Cannot read properties of null`）が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## macOS TUIフリーズの修正

Spotlightの再インデックス中にセッション開始時にmacOS TUIがフリーズ（Ctrl+C無応答）する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間アイドルセッションの履歴消失修正

別のClaude Codeプロセスが30日間のトランスクリプトクリーンアップを実行した際に、長時間アイドル中のセッションが履歴を失う問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フォアグラウンドサブエージェントの無制限ネスト修正

フォアグラウンドサブエージェントが無制限にネストチェーンを生成する問題が修正され、バックグラウンドサブエージェントと同じ5階層の深度制限が適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/recap` とモデル切り替え後のフォーク修正

モデル切り替え直後に `/recap` と会話フォークが以前のモデルを使用する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントの経過時間表示修正

サブエージェントの「Thinking」表示がサブエージェント自身の経過時間ではなく親エージェントの経過時間を表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストエージェント待機中の表示修正

ネストされたエージェントでブロックされているサブエージェントが、エージェントパネルで「waiting」ではなくティッキング経過時間を表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## APIリトライインジケーターの残留修正

APIリトライインジケーター（「Retrying in 0s · attempt N/10」）がリトライ成功後も画面に残る問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## AWS認証情報の短寿命トークン修正

AWS `awsCredentialExport` の残り寿命が短い認証情報が毎分リフレッシュされる問題が修正され、`aws configure export-credentials` のJSON形式も受け入れるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude mcp get/list` の接続ステータス修正

tools/listが失敗した場合に `claude mcp get`/`list` が `✓ Connected` と表示する問題が修正され、エラー詳細付きの `! Connected · tools fetch failed` が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/remote-control` 接続表示の修正

`/remote-control` が古い「connecting…」行を残す問題が修正され、接続完了時にトランスクリプトに確認が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsでのExitWorktreeエラー修正

bare `git` がWindows上で解決できない場合にExitWorktreeがクリーンなワークツリーの削除を「Could not verify worktree state」で拒否する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## シンボリックリンク下の設定変更修正

`~/.claude` がシンボリックリンクの場合に `~/.claude/settings.json` が相対シンボリックリンクだと設定変更（`/effort`、`/model` など）がENOENTで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## IDE選択行番号のオフバイワン修正

IntelliJとVS Codeのコンテキストリマインダーで、IDE選択の行番号が1つずれる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンでのCtrl+Cクリップボード修正

フルスクリーンでネイティブターミナル選択（modifier+ドラッグ）後にCtrl+Cがクリップボードをアプリの以前の選択で上書きする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Ctrl+Vペースト修正

クリップボードにテキストが含まれている場合にCtrl+Vがペーストではなく「No image found in clipboard」と表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows/OneDriveでのエージェント作成修正

エージェントディレクトリが既に存在する場合にエージェント作成が「EEXIST: file already exists」で失敗する問題が修正された（Windows/OneDrive）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## AskUserQuestionプレビューの折り返し修正

AskUserQuestionプレビューコンテンツがダイアログの端で切れてしまう問題が修正され、ワードラッピングが適用されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## AskUserQuestion複数選択の回答修正

AskUserQuestionの複数選択で入力した「Other」のフリーテキスト回答が送信時に無視される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/stats` タイムゾーン表示修正

`/stats` の「Most active day」と日次トークンチャートの日付がUTC負のタイムゾーンで1日早く表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Linuxクリップボードユーティリティ検出修正

`/copy` とcopy-on-selectがLinuxでClaude Code起動後にインストールされたクリップボードユーティリティを検出しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## タブインデントコードのレンダリング修正

Write（create-file）プレビューでタブインデントされたコードが不正なインデントでレンダリングされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## キューイングされたプロンプトの表示修正

ターン中にキューイングされたユーザープロンプトがトランスクリプトで全幅の背景ハイライトを表示しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Ghosttyでのスピナー表示修正

Ghosttyでアクティビティスピナーのパルスが不正なグリフサイズで停滞する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

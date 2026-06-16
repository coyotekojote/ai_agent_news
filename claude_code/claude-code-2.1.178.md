## パーミッションルールのパラメータマッチング構文

`Tool(param:value)` 構文がパーミッションルールに追加され、ツール入力パラメータを `*` ワイルドカード付きでマッチできるようになった（例: `Agent(model:opus)` でOpusサブエージェントをブロック）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストされた.claude/skillsディレクトリの読み込み

ネストされた `.claude/skills` ディレクトリ内のスキルが、そのディレクトリ配下のファイルで作業中に読み込まれるようになった。名前が衝突する場合、ネストされたスキルは `<dir>:<name>` として表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストされた.claude/ディレクトリの優先順位

agent、workflow、output-styleは作業ディレクトリに最も近い `.claude/` ディレクトリのものが優先されるようになった。project-scope workflowは最も近い既存の `.claude/workflows/` に保存される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードのサブエージェント評価改善

サブエージェントの起動が分類器によって事前評価されるようになり、サブエージェントがレビューなしでブロックされたアクションを要求できるギャップが解消された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /doctorの表示改善

`/doctor` の表示が統一されたフラットツリーレイアウトになり、セクションステータスアイコンとコマンド名のハイライトが改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフロープロンプトキーワードのハイライト変更

ワークフロープロンプトキーワードが紫のシマーハイライトに変更され、「run a workflow」や「workflow:」などの明示的なフレーズでのみトリガーされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlエラーメッセージの改善

接続失敗時にフッターに永続的な赤い「/rc failed」インジケーターが表示されるようになった。「not yet enabled」エラーがゲート、チェック失敗、古いエンタイトルメント、組織ポリシーのいずれかを説明するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /bugの改善

`/bug` が送信前に説明を必須とするようになり、モデル拒否テキストがGitHub Issueタイトルに使用されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OOMクラッシュの修正

CLIが親プロセスから古いwebsocket/OAuthファイルディスクリプタ環境変数を継承した際のメモリ不足クラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Chrome連携の修正

OAuthトークンがClaude Codeログインとは異なるアカウントに属する場合、Chrome上のClaudeが接続に失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストされたスキルのパーミッション修正

ディレクトリ修飾名を持つネストされた `.claude/skills` が非インタラクティブ実行でパーミッションプロンプトにブロックされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントの複数修正

トランスクリプト表示でツール結果とライブ進行状況が表示されるようになった。終了中のターン中に送信されたメッセージがドロップされなくなった。実行中のサブエージェントをバックグラウンド化（ctrl+b）しても最初からやり直されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## コンパクション時のフォールバックモデル修正

`--fallback-model` がコンパクション時に正しく適用されるようになり、オーバーロードまたはモデル利用不可エラー時に設定されたフォールバックモデルチェーンにフォールバックするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 認証情報キャッシュの修正

セッション外で認証情報がリフレッシュされた後、古いキャッシュされたリクエスト設定によりモデルリクエストが認証エラーで失敗し続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP disallowedToolsの修正

サブエージェントの `disallowedTools` でサーバーレベルのスペック（`mcp__server`、`mcp__server__*`、`mcp__*`）が無視される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードのundo修正

`u` がNORMAL/VISUALモードコマンドを1つずつ戻すようになり、素早い連続コマンドが1つのundoステップにマージされなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ステータスラインリンクの修正

カスタムURIスキーム（例: `vscode://`）のステータスラインリンクが `claude agents` でクリック時に開かれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## VSCode CJK IMEの修正

EscキーでCJK IME候補ウィンドウを閉じた際に実行中のClaudeタスクがキャンセルされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## マーケットプレイスプラグインのクローン修正

`CLAUDE_CODE_PLUGIN_KEEP_MARKETPLACE_ON_FAILURE=1` が新規マーケットプレイスインストールのクローンを妨げる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの修正

`/bg` または `←←` でターン終了後に作成されたバックグラウンドセッションがエージェントリストで永遠に「Working」と表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsワーカーの認証修正

カスタムAPIゲートウェイ（`ANTHROPIC_BASE_URL`、`ANTHROPIC_AUTH_TOKEN`経由）を使用するシェルからデーモンが起動された場合に、`claude agents` ワーカーが `401 Invalid bearer token` で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

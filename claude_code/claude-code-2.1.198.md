## Claude in Chromeの一般提供開始

Claude in Chromeが一般提供（GA）になった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## バックグラウンドエージェント通知フック

`claude agents`でセッションが入力を必要とする場合や完了した場合の通知フック（`agent_needs_input` / `agent_completed`）が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## バックグラウンドエージェントの自動PR作成

`claude agents`から起動されたバックグラウンドエージェントが、ワークツリーでのコード作業完了時に自動でコミット、プッシュ、ドラフトPRを作成するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## バックグラウンドエージェントの信頼性向上

長時間実行されるコマンドやワークフローが、セッションプロセスの停止・再起動・更新後も維持されるようになった。Windows環境ではバックグラウンドシェルがハンドオフされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## エージェントチームの障害処理改善

APIエラーで停止したチームメイトエージェントが「failed」をリードに報告するようになり、スタックしたチームメイトへのメッセージ送信で即座にリトライが行われるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## `/dataviz`スキルの追加

チャートやダッシュボードのデザインガイダンスを提供する`/dataviz`スキルが追加された。実行可能なカラーパレットバリデーターを含む。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## AWS上のClaude Platformプロバイダー追加

ゲートウェイプロバイダーとしてAWS上のClaude Platform（`anthropicAws`）が追加された。モデル未検出レスポンスがフェイルオーバーチェーンを進行するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## モデル継承の改善

組み込みのExploreエージェントがhaikuではなくメインセッションのモデル（opusを上限として）を継承するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## 拡張思考の継承

サブエージェントとコンテキストコンパクションがセッションの拡張思考設定を継承するようになり、委任タスクの出力品質が向上した。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## ネットワーク回復力の向上

レスポンス途中の短時間ネットワーク切断がターンを中断する問題が修正された。ECONNRESETなどの一時的エラーがバックオフ付きリトライを行うようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## バックグラウンド分類器の最適化

サンドボックスプロセスが同一ネットワークホストに繰り返しアクセスする際の過剰なバックグラウンド分類器リクエストが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## バックグラウンドタスクパネルの修正

Web、デスクトップ、VS Codeのタスクパネルで、完了後またはセッション再開後にバックグラウンドタスクが「Running」のまま停滞する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## `/diff`パネルのリフレッシュ修正

ブランチ切り替えやセッション外でのコミット時に`/diff`パネルが更新されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## Markdownテーブルのレンダリング修正

フルスクリーンモードでMarkdownテーブルがオーバーフローし右ボーダーが折り返される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## AWS認証情報の自動更新

AWS上のClaude PlatformおよびMantleセッションでSTSトークン期限切れ時に「Please run /login」で行き詰まる問題が修正された。`awsAuthRefresh`が自動実行されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## macOSローカルネットワーク権限の修正

macOSバックグラウンドエージェントセッションでローカルネットワークホストに対する「no route to host」エラーが修正された。Local Networkエンタイトルメントが宣言された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## ワークツリーディレクトリの修正

ワークツリーの入退出後に`/desktop`が「Cannot determine working directory」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## macOS再接続の修正

エージェントビュー表示中にバックグラウンドエージェントが約52秒ごとに「Reconnecting…」を繰り返し表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## エージェントアタッチ時のキーボード修正

`claude attach <id>`内で`←`キーを押すとシェルに戻ってしまう問題が修正され、エージェントビューが開くようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## 競合フラグの拒否

`claude --bg`が`--print`/`-p`と組み合わされた場合にアタッチ不可なセッションが黙って作成される問題が修正され、競合フラグが事前に拒否されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## ワークフロー進捗追跡の修正

SDKおよびデスクトップアプリセッションで、ワークフロー進捗ビューのリストから最も古いエージェントが削除される一方でフェーズカウンターは正確だった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## 条件付きルールの読み込み修正

ターゲットファイルがシンボリックリンク経由でアクセスされた場合に`.claude/rules/`の条件付きルールが読み込まれない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## フルスクリーンモードでのURL選択修正

フルスクリーンモードでのダブルクリックによる単語選択がスキームを含むURL全体を選択するように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## フルスクリーンモードでのCmd+クリック修正

macOSのWarpでフルスクリーンモード時にCmd+クリックでURLが開かない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## プランモードのツールコール修正

セッションがプランモードで開始された場合に読み取り専用ツールコールが自動許可されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## ブランチフォーク名の修正

`/branch`がコンパクションサマリーではなく最初の実際のプロンプトからデフォルトのフォーク名を導出するように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## フォーカスモードの改善

フォーカスモードが改善され、ターン中に起動されたサブエージェントがアクティビティサマリーに表示されるようになり、完了したバックグラウンド通知が単一カウントに折り畳まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## シンタックスハイライトの改善

highlight.js 11へのアップグレードにより、コードブロック、diff、ファイルプレビューのシンタックスハイライト精度が向上した。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## SSH経由のキーボードショートカットヒント

Mac上でSSH接続時のキーボードショートカットヒントがalt/superではなくopt/cmdで表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## APIリトライUXの改善

APIリトライUXが改善され、2回目の試行後にエラー理由が表示されるようになり、APIが過負荷時にスピナーヒントの代わりにステータスページリンクが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## `/login`のアクセシビリティ改善

`/login`が`claude agents`ビューから利用できないと表示する代わりにサインインダイアログを開くようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## サブエージェントメッセージの取り扱い改善

サブエージェントが起動元エージェントからのメッセージを通常のタスク指示として扱うようになった。エージェントのメッセージはユーザーの承認として扱われない。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

## `/agents`ウィザードの削除

`/agents`ウィザードが削除された。サブエージェントの作成・管理はClaudeへの依頼または`.claude/agents/`の直接編集で行う。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.198)

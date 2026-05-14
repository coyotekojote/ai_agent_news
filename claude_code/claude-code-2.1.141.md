## フックのterminalSequenceフィールド追加

フックのJSON出力に`terminalSequence`フィールドが追加され、制御ターミナルがなくてもフックからデスクトップ通知、ウィンドウタイトル、ベルを発行できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## HTTPS経由のプラグインソースクローン

`CLAUDE_CODE_PLUGIN_PREFER_HTTPS`環境変数が追加され、GitHub SSHキーがない環境でもHTTPS経由でGitHubプラグインソースをクローンできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークスペースIDによるワークロードID連携

`ANTHROPIC_WORKSPACE_ID`環境変数が追加され、連携ルールが複数のワークスペースをカバーする場合に、発行されるトークンのスコープを特定のワークスペースに限定できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントセッションのディレクトリスコープ

`claude agents --cwd <path>`でセッション一覧を特定のディレクトリにスコープできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フィードバック機能の改善

`/feedback`で最近のセッション（過去24時間または7日間）を含めて送信できるようになり、現在のセッションを超える問題の報告が可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Rewindメニューの要約機能

Rewindメニューに「Summarize up to here」が追加され、最近のターンを維持しながら以前のコンテキストを圧縮できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Autoモード権限ダイアログの改善

Autoモードの権限ダイアログで、`permissions.ask`ルールによってプロンプトが表示された場合にその旨が説明されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## IDEでのdiff表示オプションの復元

IDE接続時にファイル編集の権限プロンプトで「view diff in your IDE」オプションが復元された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントの権限モード保持

`/bg`または`←←`で起動されたバックグラウンドエージェントが、デフォルトに戻る代わりに現在の権限モードを保持するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント完了ステータスの改善

`claude agents`で作業は完了したがバックグラウンドシェルが実行中のエージェントが、Workingではなく Completedに移動するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スピナーフィードバックの改善

長い思考期間中のスピナーフィードバックが改善され、10秒後にスピナーがアンバー色に変わりClaudeがまだ作業中であることを示すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインメニューナビゲーションの改善

プラグインメニューのナビゲーションが改善され、`→`/Tabでタブ切り替え、`↑`でタブストリップへの移動、フルスクリーンモードでのタブヘッダーと検索ボックスのクリック操作が可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

バックグラウンドサイドクエリがBedrock/Vertex/Foundry/ゲートウェイで利用不可のHaikuモデルIDを送信する問題が修正され、`ANTHROPIC_SMALL_FAST_MODEL`オーバーライドが未設定の場合はメインループモデルにフォールバックするようになった。Windows上で`claude daemon status`および`/doctor`がデーモンパイプキーファイルのロック・読み取り不可時にスローする問題が修正された。`claude agents`がラッパー経由で起動された際にダッシュボードではなくエージェントタイプリストを表示する問題が修正された。作業ディレクトリが削除された際にクラッシュしたセッションを開くと冗長なディスパッチが発生する問題が修正された。カスタム`ANTHROPIC_BASE_URL`ゲートウェイ上のバックグラウンドジョブの自動命名が修正された。`/model`が他の並行セッションのautocompactしきい値を変更する問題が修正された。ツール権限プロンプト表示中の権限モード切り替えでプロンプトが自動で閉じない問題が修正された。権限・ダイアログプロンプト表示中にEnterキーが入力ボックスにもテキストを送信する問題が修正された。`EnterWorktree`後にフックが存在しない`transcript_path`を受け取る問題が修正された。マークダウンテーブルのセルラッピングがボーダーグリッドではなく縦のキーバリューレイアウトにフォールバックするリグレッション（2.1.136）が修正された。キャンセルされたプロンプトの上矢印履歴に関する複数の問題が修正された。VimのINSERT/VISUALモード中にCtrl+Cが実行中のターンを中断しない問題が修正された。`chat:submit`の代替キーバインドが`enter`を`chat:newline`に再バインドした際に動作しない問題が修正された。出力スタイル設定時にプロンプトサジェストがサイレントに無効化される問題、`spinnerVerbs`設定の無視、AskUserQuestionポップアップの表示問題、Web検索ステータスの表示問題、マルチラインステータスラインの表示問題、ライトテーマでのdiffコンテキスト行の色、エラーオーバーレイの表示問題など多数のUI・表示関連バグが修正された。Windowsでの画像ペースト、SDKのLinuxバイナリ検出、Bedrockの`awsCredentialExport`が常に実行されるよう修正された。VSCodeでのマイク表示とWSLの音声エラーメッセージが改善された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.141)

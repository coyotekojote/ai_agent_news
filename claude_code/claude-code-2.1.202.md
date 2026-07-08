## ダイナミックワークフローサイズ設定の追加

`/config`に「Dynamic workflow size」設定が追加され、Claudeがダイナミックワークフローで一般的に使用するエージェント数の規模（small/medium/large）を制御できるようになった。これはガイドラインであり、強制的な上限ではない。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## ワークフローエージェントのOpenTelemetry属性追加

ワークフローから起動されたエージェントのテレメトリに`workflow.run_id`および`workflow.name`のOpenTelemetry属性が追加され、OTelデータからワークフロー実行のアクティビティを再構成できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## Ctrl+R履歴検索のクラッシュ修正

インラインのCtrl+R履歴検索で、検索がまだ履歴ファイルをスキャン中に確定またはキャンセルした際のクラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## バックグラウンドセッションの`/rename`修正

バックグラウンドセッションに対する`/rename`がジョブの再起動時に元に戻されてしまい、新しい名前でセッションを指定できなくなる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## mTLSハンドシェイク一時的エラーの修正

クライアント証明書のインプレースローテーション中に設定が再適用された際の一時的なmTLSハンドシェイク失敗が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## Remote Controlからのコマンド送信失敗の修正

Remote Control（モバイル/Web）からインタラクティブセッションに送信されたコマンドが「Unknown command」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## Remote Controlからの画像・ファイル送信修正

Remote Controlのモバイルまたはwebアプリからキャプションなしで送信された画像やファイルが無視される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## サインインURLのクリック可能性改善

`claude auth login`および`claude mcp login --no-browser`で表示されるサインインURLが、SSH経由で折り返された際に確実にクリックできるようになった。単一のハイパーリンクとして出力されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## `claude agents`からのチャットオープン失敗修正

`claude agents`からチャットを開く際に「currently running as a background agent」エラーが発生し、その後ワーカーがクラッシュ/再起動ループに陥る問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## ワークフロースクリプトのUnicodeクォートエスケープ修正

文字列内のUnicodeクォートエスケープを含むワークフロースクリプトがパース前に破損する問題が修正された。ワークフローのパースエラーは常にTypeScriptを原因として表示するのではなく、問題のある行を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## 音声入力の無限リトライ修正

マイクまたはオーディオレコーダーが失敗した際に音声ディクテーションが無制限にリトライする問題が修正された。キャプチャの繰り返し失敗で音声入力が一時停止されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## Remote Controlの権限モード表示修正

`/remote-control`セッションがモバイルおよびwebアプリで誤った権限モードを表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## セッション再開のパフォーマンス改善

名前によるセッションの再開、または再開ピッカーの表示が、多数のgit worktreeを持つリポジトリで数分かかり大量のメモリを使用する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## インストーラー・アップデーターのダウンロード失敗修正

プロキシやネットワークがダウンロード中に接続を切断した際にインストーラーおよびアップデーターのダウンロードが即座に「aborted」で失敗する問題が修正された。一時的な接続切断はリトライされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## スキルの重複読み込み修正

既に読み込まれたスキルを再度呼び出した際に、そのインストラクションの重複コピーがコンテキストに追加される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## `/workflows`エージェントリストレイアウトの改善

`/workflows`のエージェントリストレイアウトが改善され、タイトルが広くなり、専用の時間列が追加され、モデル名が短くなり、行ごとのツールコール数が非表示になった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## MCPエラーメッセージの改善

MCPのエラーメッセージが改善され、サーバー設定に`url`があるが`type`がない場合に、誤解を招く「command: expected string」ではなく`"type": "http"`を提案するより明確なエラーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

## `/review`コマンドの変更

`/review <pr>`が高速なシングルパスレビューに戻された。選択したエフォートレベルでのマルチエージェントレビューには`/code-review <level> <pr#>`を使用する。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.202)

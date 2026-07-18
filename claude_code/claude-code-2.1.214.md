## EndConversationツールの追加

高度に悪質なユーザーやジェイルブレイク試行に対してClaudeがセッションを終了できるEndConversationツールが追加された。2025年からclaude.aiで導入されている機能と同様。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間実行ツール呼び出しの定期的な進捗ハートビート追加

以前は無音状態だった長時間実行ツール呼び出しに対して、定期的な進捗ハートビートが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## メモリファイルフロントマターへのISO `modified`タイムスタンプ追加

メモリファイルのフロントマターにISO形式の`modified`タイムスタンプが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OpenTelemetryログイベントへの属性追加

メッセージレベルの相関とツール出所のために`message.uuid`、`client_request_id`、`tool_source`属性がOpenTelemetryログイベントに追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `CLAUDE_CODE_OTEL_CONTENT_MAX_LENGTH`設定の追加

OpenTelemetryコンテンツ属性の60KB切り捨て制限を設定する`CLAUDE_CODE_OTEL_CONTENT_MAX_LENGTH`が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `subagentStatusLine`ペイロードへのreasoning effort追加

カスタムエージェント行がモデルとeffortをレンダリングできるよう、`subagentStatusLine`ペイロードにreasoning effortが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## dockerコマンドのデーモンリダイレクトフラグに対する権限プロンプト追加

`docker`コマンド（Podmanの`docker`シムを含む）で`--url`、`--connection`、`--identity`およびPodmanのリモートモードなどのデーモンリダイレクトフラグを持つコマンドに権限プロンプトが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 単一セグメント`dir/**`フック`if:`条件のマッチング変更

単一セグメントの`dir/**`フック`if:`条件が`<cwd>/dir`のみにマッチするように変更された。任意の深さでのマッチングには`**/dir/**`と記述する。`deny`/`ask`権限ルールは任意の深さのマッチを維持。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `file`コマンドの`-m`/`--magic-file`や`-f`/`--files-from`使用時の権限要求

`file`コマンドで`-m`/`--magic-file`や`-f`/`--files-from`を使用する場合、読み取り専用として自動許可されず権限が要求されるように変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## keep-alive接続プーリングのstale-connectionエラー後の無効化

stale-connectionエラー後にkeep-alive接続プーリングが無効化され、リトライ時に新しいソケットが開かれるように変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SessionStartフックのforkソース報告

セッションがフォークとして開始された場合、SessionStartフックが`"resume"`ではなく`"fork"`をソースとして報告するように変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 単一セグメント`dir/**`許可ルールの修正

`Edit(src/**)`のような単一セグメント`dir/**`許可ルールが`<cwd>/dir`のみでなく、ツリー内の任意の場所にあるネストされた`dir/`ディレクトリへの書き込みを自動承認する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows PowerShell 5.1セッションの権限チェックバイパス修正

Windows PowerShell 5.1セッションで実行されるコマンドに影響する権限チェックバイパスが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bash権限チェックのファイルディスクリプタリダイレクト形式対応

bashが権限アナライザーとは異なる方法で解析するファイルディスクリプタリダイレクト形式に対して、Bash権限チェックがクローズド（安全側）で失敗するように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非常に長いコマンドのBash権限チェック修正

10,000文字を超えるコマンドが自動実行されず、常にプロンプトが表示されるように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## zsh変数添字と修飾子のBash権限チェック修正

`[[ ]]`比較内のzsh変数添字と修飾子を不活性テキストとして扱う問題が修正され、これらのコマンドは承認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `help`と`man`コマンドの自動承認修正

安全でないオプション、コマンド置換、またはバックスラッシュパスを実行できる特定の`help`や`man`コマンドが自動承認されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートセッションの権限プロンプト修正

リモートセッションで権限プロンプトがローカル確認ダイアログの前に進行する可能性がある問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## GrowthBook機能のnull評価時クラッシュ修正

GrowthBook機能がnullに評価された場合のクラッシュと、不正な形式のフラグペイロードがキャッシュされた機能フラグを消去する可能性がある問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `pkill -f`パターンによるCLIプロセス終了修正

`pkill -f`パターンがCLI自身のプロセスに誤ってマッチした場合にBashツールがClaudeセッションを終了する問題が修正された（Linux）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--settings`によるメモリ成長問題の修正

`--settings`がデバイスファイルや数GBのファイルを指している場合の無制限メモリ成長が修正された。2MiBを超える設定ファイルは明確なエラーで起動時に失敗するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 企業プロキシ背後でのWindowsストリーミングターン失敗修正

Windowsで企業プロキシ背後での「Socket is closed」エラーによるストリーミングターンの失敗が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## stream-json出力の終了時切り捨て修正

低速リーダーのSDK/パイプラインコンシューマー向けに、終了ドレインがフラットな2秒キャップではなくキュー済みバイト数に応じてスケールするように修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スケジュールタスクの自身のプロンプト拒否修正

スケジュールタスクが自身の設定済みプロンプトを信頼できない入力として拒否する問題が修正された。発火されたプロンプトはセッションの割り当てタスクとして配信されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsでのPowerShellツールコマンドハング修正

子プロセスが標準入力を待機している場合にPowerShellツールコマンドがタイムアウトまでハングする問題が修正された（Windows）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShellツールでのPythonスクリプトUnicodeDecodeError修正

PowerShellツール配下でPythonスクリプトが標準入力から非UTF-8データを読み取る際にUnicodeDecodeErrorでクラッシュする問題が修正された（Windows）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShellツールでのPythonスクリプトUnicodeEncodeError修正

PowerShellツール経由で実行されるPythonスクリプトが非ASCII出力でUnicodeEncodeErrorでクラッシュする問題と、PowerShell 7のエラーメッセージに生のANSIエスケープシーケンスが含まれる問題が修正された（Windows）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShellツールの`where.exe`等のエラー報告修正

PowerShellツールが`where.exe`、`fc.exe`、`diff.exe`が有効な否定応答を返す場合にエラーとして報告する問題が修正された（Windows）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShellツールの`>`/`>>`によるUTF-16LEファイル書き込み修正

Windows PowerShell 5.1で`>`と`>>`がUTF-16LEファイルを書き込み、他のツールがUTF-8として読めない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドデーモンの制御ソケット削除修正

置換されたバックグラウンドデーモンがシャットダウン時に後継者の制御ソケットを削除し、次のクライアントが正常な置換デーモンを終了させる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アイドルバックグラウンドセッションのデーモン維持修正

`←`や`/background`でパークされたバックグラウンドセッションがアイドル状態のままバックグラウンドデーモンとワーカープロセスを無期限に維持する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 完了済みバックグラウンドセッションの削除不能修正

バックグラウンドサービスがアイドル状態になった後、`claude rm`やエージェントビューから完了済みバックグラウンドセッションを削除できない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非gitフォルダからのバックグラウンドセッション削除修正

非gitフォルダからディスパッチされたバックグラウンドセッションがエージェントビューから削除できない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 停止済みバックグラウンドセッションの再開時会話復元修正

セッションストアに読み取り不可能なフォルダが存在する場合に、停止したバックグラウンドセッションを再開する際に保存済み会話の復元が失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Control「session ready」プッシュ通知の誤発火修正

Remote Controlが明示的に有効化されていないセッションでRemote Controlの「session ready」プッシュ通知が発火する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューセッションでの`/install-github-app`と`/mcp`ブロック修正

エージェントビューセッションで`/install-github-app`と`/mcp`設定メニューがブロックされる問題が修正された。ターミナルが接続されていないバックグラウンドセッションでのみ拒否されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `--settings` CLIフラグで有効化されたプラグインの読み込み修正

`--settings` CLIフラグで有効化されたプラグインが読み込まれない問題が修正された（v2.1.181以降のリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間セッションでの機能フラグ失効修正

OAuthトークンのローテーション後に長時間セッションで機能フラグが古くなる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview`のマージベースなしリポジトリでの実行拒否修正

`/ultrareview`がマージベースのないリポジトリで実行を拒否する問題が修正され、全追跡ファイルのレビューを提案するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude update`と`claude doctor`のハング修正

シェル設定パスがディレクトリの場合に`claude update`と`claude doctor`がサイレントにハングし、`/status`のシステム診断セクションが空白になる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## メモリフロントマター値のインライン`#`での切り捨て修正

メモリファイル保存時にメモリフロントマター値がインラインの`#`で無言で切り捨てられる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッションコストとトークンテレメトリの二重カウント修正

複数の累積`message_delta`フレームを発信するストリームでセッションコストとトークンテレメトリが二重カウントされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アドバイザー思考中の偽「check your network」警告修正

アドバイザーが思考中に表示される偽の「check your network」警告が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 終了コード2のフックのブロック動作修正

フックのstdout JSONがスキーマ検証に失敗した場合に、終了コード2のフックがドキュメント通りにブロックしない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターンの非同期コンテキスト外のOTelログイベント修正

ターンの非同期コンテキスト外で発信されるOTelログイベントがインタラクションスパンのトレースコンテキストを欠落する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPトランジェントエラーでのスラッシュコマンドクリア修正

プロンプト/リソースリフレッシュ中のMCPトランジェントエラーがサーバーのスラッシュコマンドとリソースをクリアする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude rc`のワークスペース信頼エラーメッセージ改善

ホームディレクトリでの`claude rc`ワークスペース信頼エラーが、信頼がそこでは保存されないことを説明し、プロジェクトディレクトリからの実行を提案するように改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

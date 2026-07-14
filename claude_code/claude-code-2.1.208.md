## スクリーンリーダーモードの追加

スクリーンリーダーユーザー向けのオプトイン式プレーンテキストレンダリングが追加された。`claude --ax-screen-reader`の実行、`CLAUDE_AX_SCREEN_READER=1`の設定、またはsettingsに`"axScreenReader": true`を追加することで有効化できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## vimInsertModeRemaps設定の追加

vimモードにおいて、`jj`をEscapeにマッピングするなどの2キー挿入モードシーケンスを設定できる`vimInsertModeRemaps`設定が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CLAUDE_CODE_PROCESS_WRAPPER環境変数の追加

エージェントビューおよびバックグラウンドサービスが、すべてのClaude Codeの自己起動を企業ランチャーとして指定されたラッパー実行ファイル経由で実行する`CLAUDE_CODE_PROCESS_WRAPPER`が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンモードのマウスクリックサポート追加

フルスクリーンモードにおいて、マルチセレクトメニューと「Other」入力行へのマウスクリックサポートが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファストモード復元の修正

ファストモードをサポートするモデルに切り替えた後もファストモードがオフのままになる問題が修正され、設定で有効化されている場合は自動的に復元されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントへの返信消失修正

バックグラウンドエージェントへの返信が配信失敗時に消失する問題が修正され、テキストが保存されセッション再起動時に配信されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アップデート後のバックグラウンドセッション接続失敗修正

アップデートによってバイナリが置き換えられた後、`claude agents`プロセスからのバックグラウンドセッション接続が恒久的に失敗する問題（「Couldn't start the background daemon」）が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 自動アップデート後のコンテキストウィンドウリセット修正

CLIの自動アップデート後にコンテキストウィンドウ（および自動コンパクトインジケーター）が一時的に200kにリセットされ、長コンテキストセッション再開時に偽の「100% context used」が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## HTTP/2 GOAWAYによるクラッシュ修正

サーバーがリクエスト中にHTTP/2接続をGOAWAYで閉じた際に、管理付きセッションとバックグラウンドセッションがクラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## パイプ出力時のストリームJSON/JSON出力切り詰め修正

`claude -p`から大きなレスポンスをパイプする際にストリームJSON/JSON出力が切り詰められ、結果メッセージが欠落する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 環境変数の指数表記値修正

`CLAUDE_CODE_MAX_OUTPUT_TOKENS`および類似の環境変数が指数表記値（`1e6`が`1`になる）の仮数部を無言で使用する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 大規模Markdownテーブルのレンダリング修正

非常に大きなMarkdownテーブルがレンダリングを停止させるか過剰なメモリを使用する問題が修正され、200行を超えるテーブルは最初の200行と「… N more rows」の通知を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Editツールのファイル変更検出修正

読み取り後に変更されたファイルに対して、対象テキストがまだ一意に一致する場合でもEditツールが失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Read・Grep・Globツールの複数修正

Read がオフセット超過時に「shorter than offset」とエラー報告する問題、Grep が無効な正規表現パターンに対して無言で「No files found」を返す問題、Grep のカウントモードでページネーション時に合計が過少報告される問題、Glob がパターン・パス・作業ディレクトリにヌルバイトが含まれる場合に不明瞭なエラーでクラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## apiKeyHelperスクリプトのエラー表示修正

`apiKeyHelper`スクリプトの失敗が約10回の無言リトライ後に汎用401エラーの背後に隠される問題が修正され、3回の試行以内にスクリプト自体のエラーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrockストリーミングリクエストのエラー修正

ゲートウェイがレスポンスを変換する際にBedrockストリーミングリクエストが誤解を招く「Truncated event message received」で失敗する問題が修正され、content-typeを名前付けしプロキシを指すエラーメッセージに変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /upgradeのログインフロー表示修正

ブラウザのオープンに失敗した際に`/upgrade`がアップグレードURLの代わりにログインフローを表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsスタイルのストリームJSON入力修正

WindowsスタイルのSDKホストからの空白CRLFまたはホワイトスペースのみの行でストリームJSON入力がセッションを終了させる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ヘッドレスストリームJSONセッションのハング修正

`control_request`が非文字列の`set_model`ペイロードを運んだ際にヘッドレスストリームJSONセッションが恒久的にハングする問題が修正され、エラーレスポンスで応答するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション再開時の繰り返し通知修正

セッション再開時に繰り返し表示される「No completion record was found」通知が修正され、孤立したバックグラウンドタスクが単一のサマリーに集約されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlクライアントのバックグラウンドエージェント表示修正

ターミナルホストセッションに接続したRemote Controlクライアントが、タスクの開始または停止まで バックグラウンドエージェントとワークフローの進捗を表示しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Agentツールのツール未検出エラー修正

サブエージェントの`tools`リストが空に解決される場合にAgentツールがツールなしで起動する問題が修正され、認識されないエントリを名前付けした明確なエラーを返すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /usageおよび/mcpの表示修正

`/usage`が新しいデータの上に古いキャッシュバーを表示する問題、および`/mcp`が設定編集後にプレースホルダーサーバーを再分類しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SDKホストでのディレクトリ変更エラー修正

アイドルセッションでバックグラウンドタスクが実行中の場合に、SDKホスト（例：Claude Desktop）での「Change directory」が「A turn is in progress」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフロー保存ダイアログのパス表示修正

ワークフロー保存ダイアログがユーザースコープ保存時に`CLAUDE_CONFIG_DIR`の場所の代わりに`~/.claude/workflows/`を表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /release-notesのコンテキスト注入修正

`/release-notes`で閲覧したノートがモデルのコンテキストに追加される問題が修正された。以前は「Show all」がチェンジログ全体を後続のすべてのリクエストに注入していた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのペースト画像メモリリーク修正

ピーク返信送信後もペーストされた画像が画面の存続期間中保持されるエージェントビューのメモリリークが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SDKセッションのエージェント定義消失修正

プラグインリフレッシュがクライアント接続前に実行された場合に、初期化リクエストで定義されたエージェントがSDKセッションで失われる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間セッションの複数メモリリーク修正

長時間セッションにおける複数のメモリリークが修正された。MCP stdioサーバーのstderrがサーバーあたり最大64MBまで蓄積、LSPドキュメントが無期限にオープン（50ドキュメント上限のLRUに変更）、バックグラウンド化後の非同期フック出力の保持、ヘッドレス/SDKセッションでの大きなツール結果ペイロードによる無制限の増大が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 極長行ファイル読み取り時のメモリ肥大修正

offset/limitを使用して極端に長い単一行のファイルを読み取る際のメモリ肥大が修正され、行全体を読み込む代わりにクリーンなエラーを返すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## パーミッションルールマッチャーのキャッシュ化

多数のパーミッション拒否/確認ルールを持つセッションでのターンごとの複数秒の遅延が修正され、ルールマッチャーが一度コンパイルされキャッシュされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントタスクリスト更新時の入力応答性改善

エージェントタスクリスト更新時の入力応答性が改善され、タスク更新がUI全体を再レンダリングしなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ツールコールのCPUオーバーヘッド削減

多数のMCPツールを持つprint/SDKセッションでのツールコールごとのCPUオーバーヘッドが削減された。ツールプールアセンブリのキャッシュにより、高ツール数で最大7倍のツールラウンド高速化を実現。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファイル編集読み取りキャッシュのメモリ使用量削減

ファイル編集読み取りキャッシュが最大1,000ファイルを固定保持する代わりに16MBに制限され、メモリ使用量が削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッショントランスクリプトサイズの削減

セッショントランスクリプトサイズが削減された（編集の多いセッションで最大79倍）。また、置き換えられたファイル履歴バックアップの整理によりチェックポイントのディスク使用量が制限された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション再開時のメモリ使用量削減

大きな会話から生成されたバックグラウンドエージェントまたはフォークを持つセッションの再開時のメモリ使用量が削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 完了済みバックグラウンドエージェントの/tasks表示改善

完了したバックグラウンドエージェントが終了直後に消失せず、クリーンアップまで`/tasks`に表示され続けるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 停止済みバックグラウンドエージェントへの接続改善

停止したバックグラウンドエージェントへの接続時に、セッションのウォームアップ中に空白の「Session is starting」画面の代わりにトランスクリプトが即座に表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 旧デーモンによるワーカー再起動の防止

古いデーモンが新しいバージョンによって生成されたワーカーを古いバイナリ上で無言で再起動しなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントビューのCtrl+X動作改善

エージェントビューにおいて、Ctrl+Xがリネームされたブランチのワークツリーを削除し、プッシュされていないコミットを破壊せず、ワークツリーが保持される場合はセッション行を維持し、再利用されたワークツリー名が現在のベースにリセットされるよう改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 壊滅的削除コマンドのプロンプト追加

`$(…)`、バッククォート、`<(…)`を含むコマンド内の壊滅的な削除（例：`rm -rf ~`）が`--dangerously-skip-permissions`およびオートモードでもプロンプトを表示するようになり、プレーン形式と一致した。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションでの一部コマンド制限

`/install-github-app`と`/mcp`設定メニューがバックグラウンドセッションで開かなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 空URLのMCPサーバー表示改善

空のURLで設定されたMCPサーバーが設定エラーの代わりに`/mcp`で「not configured」と表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /usageのレート制限時表示改善

`/usage`がusageエンドポイントのレート制限時にエラー画面の代わりに「as of」の注釈付きで最後に取得した使用量バーを表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock SSO認証の修正（2.1.207リグレッション）

`sso_region`がBedrock リージョンと異なるAWS SSOプロファイルで「Session token not found or invalid」が発生しBedrock認証が失敗する問題が修正された（2.1.207のリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog)

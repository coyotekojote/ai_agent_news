## パーミッションプロファイルのデフォルト値をプロファイルとして導出

レガシー設定のデフォルト解決が、中間の `SandboxPolicy` オブジェクトを作成して変換する代わりに、`PermissionProfile` オブジェクトを直接生成するようリファクタリングされた。

[参考リンク](https://github.com/openai/codex/pull/19772)

## パーミッション: cwd 特殊パスの削除

実験的な `PermissionProfile` API から `CurrentWorkingDirectory` 特殊ファイルシステムパスが削除され、API 安定化前にパーミッションルートアクセスが `:project_roots` エントリに統合された。

[参考リンク](https://github.com/openai/codex/pull/19841)

## スレッド開始ハンドラーの整理

app-server の `thread/start` ハンドラーがリファクタリングされ、ヘルパーメソッドが `Result` 型を返すようになり、エラー処理が統合された。

[参考リンク](https://github.com/openai/codex/pull/19492)

## スレッド変更ハンドラーの整理

スレッド変更操作のエラーハンドリングが、ネストされたエラーブランチから早期リターンに置き換えられ、コードフローが直線的に改善された。

[参考リンク](https://github.com/openai/codex/pull/19493)

## codex-backend: フィルタ付きスレッドリストで state git メタデータを優先

フィルタ付きスレッドリストでの git メタデータのマージが改善され、SQLite データベースの非 null 値がファイルシステムの古い可能性のある値より優先されるようになった。

[参考リンク](https://github.com/openai/codex/pull/19874)

## exec Bazel 統合テストのシャーディング

`//codex-rs/exec:exec-all-test` 統合テストが 8 つの Bazel シャードに分割され、Windows Bazel レーンでのタイムアウト問題が解決された。

[参考リンク](https://github.com/openai/codex/pull/19862)

## スレッド読み取りハンドラーの整理

スレッド読み取り/リストハンドラーがリファクタリングされ、ビュー構築のエラーハンドリングがレスポンス出力から分離された。

[参考リンク](https://github.com/openai/codex/pull/19494)

## Python SDK の Codex バージョン固定公開

SDK パッケージが `openai-codex-app-server-sdk` として公開可能になり、SDK とランタイムパッケージが同一の Codex ランタイムバージョンに固定された。

[参考リンク](https://github.com/openai/codex/pull/18996)

## スレッドの resume/fork ハンドラーの整理

スレッド resume および fork のヘルパー関数が直接エラーを出力する代わりに `Result` 値を返すようリファクタリングされ、非同期 pending-resume の動作は維持された。

[参考リンク](https://github.com/openai/codex/pull/19495)

## キャンセルされた推論ストリームのトレース

Codex がプロバイダのレスポンスを完了前に消費停止した際にターミナルイベントを記録する機能が実装された。キャンセル前に観測された出力アイテムは保持される。

[参考リンク](https://github.com/openai/codex/pull/19839)

## ターンとリアルタイムハンドラーの整理

ターン開始、注入アイテム、ターンステアのリクエスト処理が、ネストされたバリデーションとエラーブランチの削除により簡素化された。

[参考リンク](https://github.com/openai/codex/pull/19497)

## レビューとフィードバックハンドラーの整理

レビュー、中断、ファジー検索、フィードバック、git-diff ハンドラーが整理され、バリデーション失敗が JSON-RPC エラーに変換されるようになった。

[参考リンク](https://github.com/openai/codex/pull/19498)

## MCP アプリ機能フラグの追加

`enable_mcp_apps` 機能フラグが `codex-features` レジストリに追加された。デフォルトでは無効で開発中の状態。

[参考リンク](https://github.com/openai/codex/pull/19884)

## ターミナルタイトルにアクション要求状態を表示

TUI のターミナルタイトルが、Codex がユーザーの承認または入力待ちでブロックされている際に点滅インジケーター付きのアクション要求状態を表示するようになった。設定項目が `spinner` から `activity` にリネームされた（後方互換性あり）。

[参考リンク](https://github.com/openai/codex/pull/18372)

## パーミッション: TUI スレッド状態でプロファイルを必須化

`ThreadSessionState.permission_profile` がオプションではなく必須フィールドになり、レガシーの app-server `sandbox` レスポンスが取り込み時に即座に `PermissionProfile` オブジェクトに変換されるようになった。

[参考リンク](https://github.com/openai/codex/pull/19773)

## パーミッション: SessionConfigured をプロファイルのみに変更

`SessionConfiguredEvent` から `sandbox_policy` が削除され、`permission_profile` が必須になった。古いペイロードとの互換性のためにカスタムデシリアライゼーションが追加された。

[参考リンク](https://github.com/openai/codex/pull/19774)

## パーミッション: スナップショットサンドボックスプロジェクションの導出

`ThreadConfigSnapshot.sandbox_policy` が保存フィールドから削除され、`permission_profile` と現在の作業ディレクトリからオンデマンドで導出されるようになった。

[参考リンク](https://github.com/openai/codex/pull/19775)

## パーミッション: スレッドセッションをプロファイルとして保存

`ThreadSessionState` からレガシーの `sandbox_policy` フィールドが削除され、`PermissionProfile` がキャッシュされたセッションパーミッションの唯一の権限ソースになった。

[参考リンク](https://github.com/openai/codex/pull/19776)

## app-server-protocol: パーミッションプロファイルを実験的に指定

app-server v2 で `PermissionProfile` を送信するフィールドが実験的としてマークされ、安定クライアントがこれらの不安定なワイヤフォーマット用のコードを生成することを防止する。

[参考リンク](https://github.com/openai/codex/pull/19899)

## 大規模なリモート app-server resume レスポンスの許可

WebSocket クライアントの最大フレームサイズがデフォルトの 16 MiB から 128 MiB に増加され、大規模な保存セッションがリモート TUI resume 操作中に拒否されることを防止する。

[参考リンク](https://github.com/openai/codex/pull/19920)

## アクティブターン中の /statusline と /title スラッシュコマンドの許可

`/title` と `/statusline` スラッシュコマンドがタスクのアクティブ実行中にも機能するようになった。

[参考リンク](https://github.com/openai/codex/pull/19917)

## ShutdownComplete のスレッドシャットダウン後の永続化回避

シャットダウンイベントの処理が変更され、スレッドシャットダウン後の `ShutdownComplete` メッセージのロールアウト永続化がバイパスされ、「thread not found」エラーが防止された。

[参考リンク](https://github.com/openai/codex/pull/19630)

## ゴーストスナップショットの削除

`ghost_snapshot` / `GhostCommit` が Responses API サーフェスから削除された。レガシーのゴーストスナップショットはロールアウト読み込み時にフィルタリングされ、undo 機能は失敗する代わりに利用不可を報告する。

[参考リンク](https://github.com/openai/codex/pull/19481)

## プラグイン MCP フィクスチャテストの安定化

共有の `wait_for_sample_mcp_ready` ヘルパーが追加され、MCP サーバーの起動完了前にアサーションが実行される競合状態が解消された。

[参考リンク](https://github.com/openai/codex/pull/19452)

## exec-server ファイルシステム API の codex-file-system へのリファクタリング

共有ファイルシステム型と `ExecutorFileSystem` トレイトが新しい `codex-file-system` クレートに抽出され、他のクレートが exec-server 実装に依存せずにファイルシステム抽象化を使用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/19892)

## カスタム MCP での fileparams メタデータの禁止

Codex の fileParams メタデータ処理がファーストパーティの `codex_apps` MCP サーバーに限定され、カスタム MCP サーバーがローカルパスの署名付き OpenAI ファイル参照を受信することを防止する。

[参考リンク](https://github.com/openai/codex/pull/19836)

## codex-analytics: デフォルトヘッダーにユーザーエージェントを追加

標準の Codex User-Agent ヘッダーが共有デフォルトヘッダーに追加され、responses-api の WebSocket ハンドシェイクが HTTP リクエストと同じクライアント OS およびバージョン情報を持つようになった。

[参考リンク](https://github.com/openai/codex/pull/17689)

## エージェントアイデンティティランタイムの即時ロード

AgentIdentity 認証がモデルプロバイダ呼び出し用に、遅延ロードではなく認証ロード時にランタイムプロセスタスクを登録するようになった。

[参考リンク](https://github.com/openai/codex/pull/19763)

## PR テンプレートの招待要件の明確化

PR テンプレートが更新され、外部コード貢献が招待制であることが明確化され、`docs/contributing.md` への参照が追加された。

[参考リンク](https://github.com/openai/codex/pull/19912)

## リモートプラグインアンインストール API の追加

必須の `pluginId` とオプションの `remoteMarketplaceName` を使用するリモート `plugin/uninstall` リクエストハンドラーが実装された。バックエンドの検証、ローカルキャッシュ削除、キャッシュクリアを含む完全なワークフローが追加された。

[参考リンク](https://github.com/openai/codex/pull/19456)

## リモートプラグインバンドルのインストール時キャッシュ

リモートインストールがプラグインバンドルをローカルにフェッチ、検証、ダウンロード、キャッシュするようになった。

[参考リンク](https://github.com/openai/codex/pull/19914)

## `codex update` コマンドの追加

トップレベルの `codex update` サブコマンドが実装された。以前は「codex update」を実行すると「update」をプロンプトとする対話セッションが開始されていた。既存のインストールチャネル検出とアップデートコマンド機能を再利用している。

[参考リンク](https://github.com/openai/codex/pull/19933)

## MultiAgentV2 ルート・サブエージェントコンテキストヒントの追加

MultiAgentV2 セッションがロール固有のスタートアップガイダンスを受け取るようになった。ルートスレッドはルート固有のヒントを、サブエージェントスレッドはサブエージェント固有のヒントを受け取る。サブエージェントが親履歴をフォークする際にヒントに一致する開発者メッセージは除外される。

[参考リンク](https://github.com/openai/codex/pull/19805)

## メモリ機能の分割（パート 2）

メモリ機能のコアモジュールからの抽出が継続され、書き込みトリガーメカニズムが app-server レベルに移動された。コアモジュールが `codex-memories-write` から完全に独立するようになった。

[参考リンク](https://github.com/openai/codex/pull/19860)

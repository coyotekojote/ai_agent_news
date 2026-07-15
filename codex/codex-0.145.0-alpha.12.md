## TUIステータス表示のストリーム出力周辺の修正

確定済みのアシスタント出力がトランスクリプトにコミットされた際に作業中ステータスインジケーターが非表示になるようになった。タスク実行中に画像生成が開始された際にはステータスが復元される。

[参考リンク](https://github.com/openai/codex/pull/33105)

## 特殊ファイルシステムサブパスの文字列保持

特殊ファイルシステムサブパスがコア権限モデルで文字列として保存されるようになり、相対パスや他プラットフォームのパス表記の誤解釈が回避された。

[参考リンク](https://github.com/openai/codex/pull/33107)

## ページネーションされたスレッドのフォーク拒否

ソーススレッドの `history_mode` がチェックされ、ページネーションされたソーススレッドに対する `thread/fork` がmethod-not-foundエラーを返すようになった。

[参考リンク](https://github.com/openai/codex/pull/33109)

## Codex Appsツールキャッシュの注入サポート

`ThreadManager` 構築時に呼び出し元が提供する `CodexAppsToolsCache` が受け付けられるようになった。インメモリランタイム用の `ConnectorRuntimeManager::new_without_cache()` も追加された。

[参考リンク](https://github.com/openai/codex/pull/33113)

## GPT-5.6プロンプトガイダンスとマイグレーション案内の改善

`text.verbosity` がデフォルトのレスポンス詳細制御として文書化され、GPT-5.6向けのプロンプトガイドラインが明確化された。

[参考リンク](https://github.com/openai/codex/pull/33121)

## モデルカタログ権限メッセージのサポート

サンドボックスモードごとの権限メッセージが `ModelMessages` に追加され、アクティブなネットワークポリシーに対する `{{ network_access }}` の置換がサポートされた。

[参考リンク](https://github.com/openai/codex/pull/33147)

## ルータープランニング前のMCPツールランタイム構築

フィルタリングされたMCPツールメタデータが、ツールルーター構築前に `CoreToolRuntime` インスタンスに変換されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33149)

## Windowsでのexec yield タイミングの明確化

Windowsにおける `yield_time_ms` が、実行中のコマンドがセッションIDを返すまでの最大待機時間として記述された。10秒のデフォルトが推奨される。

[参考リンク](https://github.com/openai/codex/pull/33150)

## app-serverリストAPIでのページネーションスレッド履歴サポート

ページネーションされたスレッドの `thread/turns/list` がスレッドストアを経由してルーティングされ、カーソル、ソート方向、ターンステータス、タイミングが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33152)

## 起動プリウォームタスクのトレース追加

WebSocket起動プリウォームにトレーススパンが付与され、セッションの `thread.id` がアタッチされるようになった。

[参考リンク](https://github.com/openai/codex/pull/33155)

## デタッチドレビューのレビューエージェントターン化

読み取り専用で欠陥優先のレビューガイダンスを持つバンドル `$review-agent` スキルが追加された。デタッチドレビューが `AgentRunner` を通じて開始されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33156)

## スリープアイテムの拡張機能ライフサイクルパスへの移動

`SleepItem` が `codex-extension-items` で定義され、`clock.sleep` イベントが `TurnItem::Extension` を通じて伝達されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33159)

## Noise環境接続の登録時まで遅延

保留中のWebSocket URL登録が、明示的な準備完了シグナルで接続をゲートする遅延Noise環境登録に置き換えられた。

[参考リンク](https://github.com/openai/codex/pull/33166)

## Windowsのexec yieldタイム範囲の文書化

Windowsにおける `exec_command.yield_time_ms` の有効範囲が2,000〜30,000msとして文書化された。

[参考リンク](https://github.com/openai/codex/pull/33167)

## app-serverでのAmazon Bedrockログインサポート

`type: "amazonBedrock"` による実験的な `account/login/start` が処理されるようになった。APIキーとMantleリージョンの検証、認証情報の永続化、プロバイダー選択が実装された。

[参考リンク](https://github.com/openai/codex/pull/33170)

## GPT-5.4からGPT-5.6バリアントへのマイグレーション

`gpt-5.4` および `gpt-5.4-mini` がモデル選択から非表示にされ、それぞれ `gpt-5.6-terra` および `gpt-5.6-luna` への移行が案内されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33173)

## ログアウト時のAmazon Bedrock認証情報処理

ログアウト時にマネージドBedrockキーが削除されるようになった。AWS管理の認証情報が誤って表現されることはない。

[参考リンク](https://github.com/openai/codex/pull/33175)

## Guardianポリシープロンプト用モデルカタログテンプレートサポート

Guardianの指示を構築するためのオプションの `policy_template` が自動レビューモデルメッセージに追加された。

[参考リンク](https://github.com/openai/codex/pull/33177)

## 同時MCP stdin書き込みの直列化

エグゼキュータベースのMCP stdio送信が単一許可セマフォでガードされ、重複書き込みが防止されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33180)

## インポート時のプラグインインストール失敗サブタイプの保持

外部エージェント設定インポート失敗に `subErrorType` が追加され、通知とアナリティクスを通じて伝達されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33182)

## MCPツールカタログのセッション間再利用

一致するstdio MCPサーバーの最近のツールカタログがキャッシュされ、新しい接続がバックグラウンドで開始される間にカタログが提供されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33184)

## 承認テストターゲットの一時ホームへの配置

承認テストターゲットが、プロセスの作業ディレクトリではなくテストの一時ホームからの相対パスで解決されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33185)

## レート制限処理でのワークスペース支出制御の尊重

`spendControlReached` 状態がレート制限スナップショットとapp-serverプロトコルを通じて伝播され、スパースアップデート間でも保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33187)

## 0.123.0-alpha シリーズ概要

0.122.0 の安定版リリース後、0.123.0-alpha.1 から 0.123.0-alpha.9 まで 9 つのアルファプレリリースが 2026 年 4 月 20〜22 日にかけて公開された。個別のリリースノートは提供されていないが、コミット履歴から以下の変更が確認されている（131 コミット、835 ファイル変更）。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## Guardian / Auto-Review システム（新機能）

エージェントアクションの自動セキュリティレビューを行う Guardian / Auto-Review システムが追加された。Auto-Review ポリシー設定、ショートサーキットロジック、保存された Auto-Review 拒否の承認機能が実装された。Guardian ネットワーク承認トリガーコンテキスト、TTFT（最初のトークンまでの時間）プランビング、トランケーション処理、分析イベント発行も追加された。TUI でのガーディアンポリシー設定デバッグもサポートされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## パーミッションプロファイルとセキュリティ

スレッド/セッション単位の詳細なパーミッション制御インフラストラクチャが追加された。app-server でのパーミッションプロファイルオーバーライドの受け入れ・スレッドパーミッションプロファイルの公開、アクティブパーミッションプロファイルの導出、exec-server でのファイルシステムサンドボックスプロファイルの運搬と arg0 エイリアスルートの公開が実装された。MCP パーミッションポリシー同期の修正、Windows でのサンドボックス用長寿命セッションの使用、明示的な AgentIdentity 認証モードの追加も行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## プラグイン・スキルシステムの改善

リモートプラグインのリスト表示・読み取りがサポートされた。コンテキストバジェット内でスキル説明を公平にトリムする機能、ブラウザ要件フィーチャーキーの登録、画像生成システムスキルの更新が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## インフラストラクチャとプラットフォーム

executor HTTP リクエストランナーの実装、公開可能な Python ランタイムホイールのステージング、フィルタ済みスレッドリスト用のオーバーレイ状態 DB git メタデータ、スレッドリストの複数 cwd フィルターサポートが追加された。非同期 main 中の arg0 ディスパッチエイリアスの維持、Windows CI スイートのシリアライズ、未使用の Bedrock 認証遅延ローディングの削除も行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## TUI の修正

リモート app-server イベントのドレイン維持、TUI ステータスサーフェスの同期維持、リモート app-server シャットダウンレースの修正、キューされたメールボックスメールの wait_agent タイムアウト修正が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

## 分析・テレメトリ

コアセッションのロールアウトトレース記録、メモリの A/B テスト準備が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.123.0-alpha.9)

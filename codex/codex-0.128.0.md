## 永続的な /goal ワークフローの追加

永続的な `/goal` ワークフローが追加された。app-server API、モデルツール、ランタイム継続、および TUI コントロール（作成、一時停止、再開、クリア操作）が含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## codex update コマンドの追加

トップレベルの `codex update` コマンドが実装された。以前は「codex update」を実行するとプロンプトとして解釈されていたが、専用のサブコマンドとして動作するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## TUI キーマップの設定対応

TUI のキーマップが設定可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## プランモードのナッジとアクション要求ターミナルタイトル

プランモードのナッジ機能が追加され、ターミナルタイトルにアクション要求状態が表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## アクティブターン中の /statusline と /title 編集

`/statusline` および `/title` スラッシュコマンドがタスクのアクティブ実行中にも編集可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## パーミッションプロファイルの拡張

パーミッションプロファイルがビルトインデフォルト、サンドボックス CLI プロファイル選択、カレントディレクトリ制御で拡張された。クライアント向けのアクティブプロファイルメタデータも提供されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## プラグインワークフローの改善

マーケットプレイスインストール、リモートバンドルキャッシュ、リモートアンインストール、プラグインバンドルフック検出、フック有効化状態の永続化、外部エージェント設定インポートがサポートされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## 外部エージェントセッションインポート

外部エージェントセッションのバックグラウンドインポート機能とインポートセッションのタイトル処理が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## MultiAgentV2 設定の明示化

MultiAgentV2 のスレッドキャップ、待機時間制御、ルート/サブエージェントコンテキストヒント、バージョン固有の深度処理が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## バグ修正

- スタックした割り込みハングおよびスレッド再開時の永続化プロバイダ復元が修正された
- 大規模なリモート resume レスポンスの処理が改善された
- ターミナルリサイズのリフロー、Markdown リストの間隔、スラッシュコマンドポップアップのレイアウトなど TUI の信頼性が向上した
- マネージドネットワークの遅延拒否処理、プロキシバイパスデフォルト、IPv6 ホストマッチングが強化された
- Windows サンドボックスおよび PTY のエッジケース（疑似コンソール起動、昇格ランナープロセス処理）が修正された
- Bedrock モデルの `apply_patch` サポートおよび GPT-5.4 推論レベルが修正された
- MCP/プラグインの stdio サーバークリーンアップおよび承認永続化のエッジケースが修正された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

## ドキュメントとメンテナンス

- バンドル済み OpenAI Docs スキルが GPT-5.5 および `gpt-image-2` 対応に更新された
- `codex-app-server` リリースアーティファクトが公開された
- `--full-auto` フラグが非推奨となり、明示的なパーミッションプロファイルへの移行が推奨されるようになった
- Python app-server SDK の Codex 固定バージョニングが実装された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.128.0)

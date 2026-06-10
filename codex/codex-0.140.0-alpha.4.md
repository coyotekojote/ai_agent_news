## 破損したSQLiteデータベースからの自動復旧

破損したSQLiteデータベースが検出された場合に自動復旧が行われるようになった。データ破損によるセッション喪失のリスクが低減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## App-serverバックグラウンドターミナルプロセスAPI

App-serverにバックグラウンドターミナルプロセスAPIが追加された。バックグラウンドでのターミナルプロセス管理が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## App-serverスレッド削除API

App-serverに`thread/delete` APIが追加され、スレッドの削除がプログラマティックに行えるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## App-server再帰制限の引き上げ

App-serverの再帰制限が引き上げられ、より深いネストのリクエストを処理できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## ブロッキング外部エージェント移行フローの削除

ブロッキングされていた外部エージェント移行フローが削除され、移行プロセスが簡素化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## 無効化されたMCPサーバーのランタイムオーバーレイ間保持

無効化されたMCPサーバーがランタイムオーバーレイを跨いで保持されるようになった。設定の一貫性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## リモートプラグインのローカル探索スキップ

リモートプラグインに対してローカルのキュレーション探索がスキップされるようになり、プラグイン検出の効率が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## Plugin-service MCPのホスト型プラグインランタイム化

Plugin-service MCPがホスト型プラグインランタイムとして使用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## 子MCPの警告が親トランスクリプトから分離

子MCPの警告が親トランスクリプトに表示されなくなり、ログの明瞭性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## MCP接続起動のフォールバック対応

MCP接続の起動がfallibleになり、接続失敗時の処理が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## アーカイブロールアウト検索のCPU削減

アーカイブロールアウト検索のCPU使用量が削減され、パフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## WindowsリリースのLLDリンク

WindowsリリースがLLDでリンクされるようになり、ビルドパフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## マルチエージェントスポーンメトリクスのバージョンタグ

マルチエージェントスポーンメトリクスにバージョンタグが付与されるようになり、エージェント生成の分析が改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## 外部エージェントインポート機能の追加

`/import`コマンドが追加され、外部エージェントのインポートが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

## 再利用可能なOTELゲージ計器の追加

再利用可能なOTELゲージ計器が追加され、メトリクス収集の効率が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.140.0-alpha.4)

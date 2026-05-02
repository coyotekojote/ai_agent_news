## メトリクス整合性と標準化レポートの実装

メトリクスの整合性チェックと標準化されたレポート機能（BT-01）が実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26240)

## /commands に list サブコマンドを追加

`/commands` コマンドに `list` サブコマンドが追加され、利用可能なコマンドの一覧表示が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/22324)

## /extensions uninstall のエイリアスとして delete を追加

`/extensions uninstall` の代替として `delete` コマンドが使用可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/25660)

## 音声モードの UI 改善

音声モード用のマイクアイコンとプレースホルダーテキストが更新された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26270)

## バグ修正

- 自動アップデートチェックで解決済みサンドボックス状態が正しく使用されるようになった
- GEMINI.md パスがディレクトリの場合にサイレントスキップされるようになった（EISDIR エラーの防止）
- 非インタラクティブなプログラムモードで `AgentExecutionBlocked` が正しくレポートされるようになった
- レガシーファイルのセッション削除時にツール出力が適切にクリーンアップされるようになった
- JSON 出力への情報ログの汚染が防止された

[参考リンク](https://github.com/google-gemini/gemini-cli/commits/main/?since=2026-04-30&until=2026-05-01)

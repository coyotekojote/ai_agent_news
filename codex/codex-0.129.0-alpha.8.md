## プロキシ Egress 診断

ローカルプロキシ経由の Git トラフィックに対する可観測性が追加された。HTTP/CONNECT トラフィックルーティング、アップストリームダイアルタイミング、CONNECT フォワーディングライフサイクルイベントがログに記録される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## TUI Raw スクロールバックモード

`/raw [on|off]` コマンドと `tui.raw_output_mode` 設定が導入された。デフォルトで Alt-R にバインドされ、折り返しテキストやパラグラフの選択が困難な粒度のコピー問題が解決された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## persistExtendedHistory の非推奨化

ロールアウトファイルに過剰なデータを永続化するスケーラビリティの問題を解消するため、`persistExtendedHistory` パラメータが非推奨化された。`thread/start`、`thread/resume`、`thread/fork` に影響。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## ツールアイテムイベントスキーマ

コマンド実行、ファイル変更、MCP コール、画像生成のイベントスキーマが定義された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## プロセスツールの環境選択ルーティング

複数の環境が存在する場合にシェルスタイルツールがターゲット環境を特定できるようになった。`include_environment_id` スキーマオプションが追加され、プロセスツールにスコープが限定された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## フック信頼メタデータと強制

未管理のフックがレビューされるまで実行されないことを防ぐ共有バックエンド信頼モデルが実装された。`config.toml` に `trusted_hash` が永続化され、`hooks/list` 経由で `currentHash` と `trustStatus` が公開される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## JSON-RPC エラーヘルパーの共有化

手動の JSON-RPC エラーオブジェクト構築が `internal_error()`、`invalid_request()`、`invalid_params()` の共有ヘルパーに統合された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## TurnItemsView の追加

`TurnItemsView` 列挙型が導入され、`notLoaded`、`summary`、`full` バリアントにより空のアイテム配列がデータの不在か意図的な未ロードかが明確化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

## /diff コマンドのワークスペースコマンド経由化

`/diff` がリモートセッション向けに直接ローカル実行ではなく app-server 経由でルーティングされるようになった。呼び出し元設定のタイムアウトと出力上限なしオプションが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.8)

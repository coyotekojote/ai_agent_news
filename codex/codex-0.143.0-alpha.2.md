## esbuild の 0.28.1 へのアップデート

Deno バイナリダウンロードに影響するセキュリティ脆弱性 GHSA-gv7w-rqvm-qjhr に対応するため、esbuild が 0.28.1 にアップデートされた。

[参考リンク](https://github.com/openai/codex/pull/29489)

## プラグインのダークモードロゴメタデータ追加

プラグインインターフェースにダークモードロゴサポートのための `logoDark` と `logoUrlDark` フィールドが追加された。

[参考リンク](https://github.com/openai/codex/pull/29488)

## 環境コンテキストのモデルワールドステートへの移行

環境コンテキストが型付き `WorldState` コンテナにリファクタリングされ、決定論的なレンダリングと差分サポートが実現された。

[参考リンク](https://github.com/openai/codex/pull/29249)

## トークンバジェットウィンドウコンテキストのラッピング

トークンバジェットの初期コンテキストが `<context_window>` タグで明示的に囲まれるようになった。

[参考リンク](https://github.com/openai/codex/pull/29494)

## リモート画像 URL のエラーテキスト置換

HTTP(S) 画像 URL がエラーメッセージに置換され、データ URL のハンドリングは維持された。

[参考リンク](https://github.com/openai/codex/pull/29417)

## レスポンスアイテムメタデータへの turn_id 保存

永続化追跡のため、ターン中に耐久性のあるレスポンスアイテムに `turn_id` が割り当てられるようになった。

[参考リンク](https://github.com/openai/codex/pull/28360)

## MCP ツールのツール検索デフォルト化

サポートされている場合、MCP ツールのツール検索が無条件で有効化され、以前のフィーチャーフラグ依存が削除された。

[参考リンク](https://github.com/openai/codex/pull/29486)

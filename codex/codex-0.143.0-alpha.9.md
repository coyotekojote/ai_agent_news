## 代替された MCP マネージャーのリフレッシュ時シャットダウン

MCP マネージャーのリフレッシュ時に、古いマネージャーが drop に依存せず明示的にシャットダウンされるようになった。

[参考リンク](https://github.com/openai/codex/pull/29608)

## インラインコンパクションでのターン所有ワールドステート使用

`run_turn` が現在の状態を所有することで、コンパクションがモデルに見えるのと同じワールドステートを使用するようになった。

[参考リンク](https://github.com/openai/codex/pull/29527)

## ロールアウト永続化メトリクスの additional_tools 対応

`ResponseItem::AdditionalTools` がレスポンスメトリクスラベルにマッピングされ、リリースビルドのコンパイルエラーが修正された。

[参考リンク](https://github.com/openai/codex/pull/29672)

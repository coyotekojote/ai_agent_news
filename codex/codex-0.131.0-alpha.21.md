## app-server画像入力のdetail保持

app-serverの入力で画像のdetailパラメータが保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## リモートコントロールAPIのUX改善

app-serverのリモートコントロールAPIが改善され、より使いやすいインターフェースが提供されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## リモートコンパクションv2のサポート

リモートコンパクションv2で`compaction_trigger`アイテムが使用されるようになり、compactフックが実行されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## プロファイルでのワークスペースルートサポート

権限プロファイルでワークスペースルートがサポートされるようになり、サマリーに有効なワークスペースルートが表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## MCPターンメタデータの拡張

MCPターンメタデータに`user_input_requested_during_turn`フィールドが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## MCP製品SKUの転送

Codex設定からapps MCP製品SKUが転送されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## バグ修正

SQLiteメタデータ同期失敗が緩和された。gitヘルパーで設定済みフックが無視されるようになった。`/side`がEscキーで閉じたり巻き戻されたりしなくなった。ローカルstate DB起動失敗からの回復が改善された。`/review`モードのMCP起動レンダリング問題が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.21)

## セーフティバッファリング処理メタデータの伝播

HTTP レスポンスヘッダーと WebSocket メタデータからセーフティバッファリング処理が読み取られ、`showBufferingUi` と `fasterModel` がアプリサーバー通知を通じて伝播されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29473)

## PowerShell の未低下 AST 領域の拒否

Windows の PowerShell セーフコマンド分類器が強化され、パラメータデフォルト、名前付きブロック、using プリアンブル、trap ハンドラーなど実行可能な AST コンテンツを含むスクリプトが拒否されるようになった。

[参考リンク](https://github.com/openai/codex/pull/24092)

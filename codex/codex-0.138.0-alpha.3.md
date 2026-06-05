## スタンドアロン画像生成の保存パスヒント

スタンドアロン画像生成のツール出力にデフォルト保存パスのヒントが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

## 外部エージェントセッション検出の高速化

パース対象が直近50セッションに制限され、検出時間が95.8%削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

## プラグインリストのマーケットプレイスソース表示

プラグインリストのJSON出力に設定済みマーケットプレイスソースのメタデータが含まれるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

## app-serverの設定オーバーライド

app-serverスタンドアロンバイナリで`-c`フラグによる設定オーバーライドが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

## コードモードのツール名前空間除外

コードモードインターフェースから特定のツール名前空間を選択的に除外できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

## バグ修正・改善

MCP移行時の無効なstdio/HTTP混在設定が防止されるようになった。

フォークされたスレッドのIDが分析初期化時に送出されるようになり、スレッド系譜の追跡が可能になった。

Windowsリリース署名がAzureアーティファクト資格情報に更新された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.3)

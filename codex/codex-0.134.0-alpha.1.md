## `codex mcp add`でのOAuthオプションサポート

`codex mcp add`コマンドでOAuthオプションがサポートされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## `codex sandbox`の`--profile`オプション対応

`codex sandbox`コマンドで`--profile`オプションが利用可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## ホストサンドボックスバックエンドの自動推論

サンドボックスのバックエンドが自動的に推論されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## readOnly注釈によるMCPツールの並列呼び出し対応

`readOnly`と注釈されたMCPツールが並列で呼び出せるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## 大規模なツールスキーマのベストエフォートコンパクション

大規模なツールスキーマに対してベストエフォートのコンパクションが行われるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## マネージドネットワークプロキシのNode envプロキシ対応

マネージドネットワークプロキシ環境でNode envプロキシが有効化されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## レガシープロファイル設定の削除

レガシープロファイルのv1解決パス、書き込みパス、使用テレメトリ、app-serverのレガシープロファイル設定が削除された。`--profile`使用時にはマイグレーションガイダンスが表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

## バグ修正

TUIレンダリング前にWindows VTが復元されるようになった。レガシープロファイルセレクターが正しくリジェクトされるようになった。app-serverのオプショナルboolアノテーションが修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.134.0-alpha.1)

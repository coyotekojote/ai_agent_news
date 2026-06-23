## OTEL へのサービスティアと推論エフォート公開

`service_tier` と `model_reasoning_effort` が OTEL ロギングに追加された。

[参考リンク](https://github.com/openai/codex/pull/29155)

## リモートコンパクション結果ハンドリングのリファクタリング

リモートコンパクション結果のハンドリングが網羅的マッチにリファクタリングされ、`TurnAborted` パスが保持された。

[参考リンク](https://github.com/openai/codex/pull/29068)

## 冗長な Codex Apps マネージャーフラグの削除

有効サーバーマップを使用することで `McpConnectionManager` の重複状態が排除された。

[参考リンク](https://github.com/openai/codex/pull/29518)

## Responses Lite のインプットアイテム使用への切り替え

Responses Lite がトップレベルツールの代わりに `additional_tools` とデベロッパーアイテムを使用するように切り替えられた。

[参考リンク](https://github.com/openai/codex/pull/27946)

## Codex Apps クライアントハンドリングの集中化

Codex Apps サーバーの分類が `AsyncManagedClient` 作成時に一度だけ行われるようになり、単一の信頼できる情報源となった。

[参考リンク](https://github.com/openai/codex/pull/29528)

## 画像 URL バリデーションの additional_tools 対応

`ResponseItem::AdditionalTools` を処理するようバリデーションが更新され、コンパイルエラーが防止された。

[参考リンク](https://github.com/openai/codex/pull/29577)

## 冗長な Codex Apps キャッシュガードの削除

キャッシュヘルパーの重複サーバー名チェックが排除され、`write_codex_apps_tools_cache` にリネームされた。

[参考リンク](https://github.com/openai/codex/pull/29575)

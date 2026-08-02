## キャパシティ枯渇のターミナルエラー分類

キャパシティ枯渇エラーがターミナル（終端）エラーとして分類されるようになり、リトライのハングが防止されるようになった。従来はキャパシティ制限に達した際にリトライロジックが繰り返し実行されてハングする問題があった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.55.0-nightly.20260801.gf47d6c6f7)

## InvalidStreamErrorの詳細をUIに伝播

`InvalidStreamError`の詳細情報がUIに伝播されるようになり、空のレスポンスが返された際にユーザーに具体的なガイダンスが表示されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.55.0-nightly.20260801.gf47d6c6f7)

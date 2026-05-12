## マルチ環境apply_patchサポート

複数環境にわたる`apply_patch`のルーティングが追加された。フリーフォームとfunction-callの両方のツールフローで環境IDがランタイムおよび承認サーフェスに伝搬される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.9)

## 起動およびTTFTテレメトリ

`codex.startup_phase`のOTelイベントが導入され、スレッド作成、プレウォームコンテキスト構築、ツール/プロンプト構築、WebSocketウォームアップなどの各フェーズが追跡されるようになった。既存メトリクスを維持する`codex.turn_ttft`イベントも追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.9)

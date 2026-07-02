## リクエスト単位のTTFTテレメトリ

推論リクエストごとのTime-to-First-Token（TTFT）テレメトリが実装された。レスポンスストリーム開始時にタイマーが起動し、最初の出力アイテムでラッチされ、`ttft_ms`がテレメトリレコードに付加される。既存のターンレベルメトリクスとは区別され、隠れた推論開始時間がキャプチャされる。

[参考リンク](https://github.com/openai/codex/pull/30883)

## Bedrockモデル可用性メタデータの修正

Amazon BedrockのGPTモデルカタログにおけるメタデータの継承問題が修正された。クローンされたGPT-5.6バリアントがGPT-5.5から`availability_nux`と`upgrade`フィールドを引き継いでいた問題が解消された。

[参考リンク](https://github.com/openai/codex/pull/30897)

## quick-xmlの脆弱性解決

quick-xml 0.38.4に影響するDoSセキュリティアドバイザリ（RUSTSEC-2026-0194、RUSTSEC-2026-0195）に対処し、quick-xmlがバージョン0.41.0にアップグレードされた。

[参考リンク](https://github.com/openai/codex/pull/30941)

## インクリメンタルリクエストのWebSocketメタデータ処理

リクエストデータと以前のレスポンスを比較する際にメタデータが無視されるようになり、インクリメンタルリクエストの成功率が向上した。

[参考リンク](https://github.com/openai/codex/pull/30770)

## ツールコールタイミングの構造化テレメトリ

直接ツールコール実行のタイミングに関する構造化JSONログが追加された。ディスパッチ待機時間とハンドラー実行時間が分離され、`codex.tool_call`完了イベントに会話、ターン、ツール、コール、トレース、タイミングフィールドが含まれる。

[参考リンク](https://github.com/openai/codex/pull/30334)

## v2レジューム時の子孫再読み込み回避

v2ルートレジューム時に永続化された子孫スレッドが即座に再読み込みされなくなった。アイドル状態の「Interrupted」v2レジデントがスロット枯渇を防ぐためにエビクション対象として扱われるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## 外部ツール出力のメモリ除外

ツール出力に`contains_external_context()`メソッドが追加された。スタンドアロンWeb検索の出力が外部コンテキストとして分類され、無効化時に外部ツールがメモリに影響を与えないようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## リリースシンボルアーティファクトの復元

macOS、Linux、Windows向けに別々のシンボルアーカイブが再構築された。フルデバッグ情報の代わりに「line-tables-only」デバッグ情報が使用され、ビルドが高速化された。配布バイナリはストリップされ、Windows PDBは保持される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## ブロッキング接続クリーンアップの回避

接続処理においてRPCクロージャーとドレインが分離された。スタックしたRPCがトランスポートイベント処理をブロックしなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## Responsesクライアントメタデータへのウィンドウid追加

Responsesの`client_metadata`フィールドにウィンドウIDが含まれるようになった。リモートコンパクションv2リクエストがサポートされる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## コンパクション分析の詳細レポート

保持画像数とコンパクションサマリートークンのNullableフィールドが追加された。詳細は`responses_compaction_v2`の場合のみ記録される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## 外部エージェントセッションインポートの高速化

インポートされたセッションがライブスレッドを開始する代わりにThreadStoreを通じて直接永続化されるようになった。5セッション制限のパイプラインで処理され、50セッションフィクスチャで約12倍のパフォーマンス改善（70秒から6秒）が達成された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## マーケットプレイスソースの公開

CLIマーケットプレイスリスト出力に`marketplaceSource`フィールドが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## カスタムランナー名のテンプレート化

ハードコードされた「codex」ランナー参照がリポジトリ名テンプレートに置き換えられた。異なるリポジトリコピー間でのワークフローの移植性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## オートレビューの設定・委譲間での保持

レビュアーIDがプロトコル間で一貫して「auto_review」としてシリアライズされるようになった。レガシーの「guardian_subagent」入力との後方互換性が維持される。スポーンされたエージェントに有効な承認レビュアーが伝播される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

## マルチエージェントv2使用プロンプトの調整

デフォルトの使用ヒントがローカル作業を優先するよう絞り込まれた。spawn_agent関数の説明にプリコールゲートが追加され、独立した境界のある並列化可能なサブタスクに焦点が当てられた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.8)

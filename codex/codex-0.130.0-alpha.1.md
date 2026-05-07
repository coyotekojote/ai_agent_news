## プラグインフックの詳細表示

`plugin/read` がバンドルされたフックのフックサマリーを含むように拡張され、プラグイン詳細ビューにフック行が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## ビルトイン MCP のファーストクラスランタイムサーバー化

プロダクト所有のビルトインが設定ベースの MCP サーバーから分離された。ビルトインは stdio サブコマンドの代わりに非同期トランスポートを介してインプロセスで起動されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## ターン差分追跡のオペレーションバック化

ファイルシステムベースのターン差分追跡がオペレーションベースのアキュムレータに置き換えられた。移動上書きケースの検証済み apply_patch 状態が保持される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## フィードバックアップロードへのアカウント ID 追加

認証由来の `account_id` がフィードバックタグに出力されるようになり、複数の ChatGPT ワークスペース間でのフィードバックトリアージが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## apply_patch 部分失敗時の正確なターン差分保持

エラー時にコミット済みプレフィックスを含む `ApplyPatchFailure` が返されるようになり、試行間でコミット済みデルタが蓄積されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## ツールレビューイベントスキーマの追加

`ReviewEvent` 分析エンベロープが定義され、レビュー対象、レビュアー、トリガー、ステータスの enum が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## プラグイン共有メタデータの公開

`PluginSummary.shareContext` に shareUrl とリーダーターゲットが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

## バグ修正

- `PluginListParams` テストイニシャライザに必須の `marketplace_kinds` フィールドが追加された
- 未使用のデバイスキークレートが削除された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0-alpha.1)

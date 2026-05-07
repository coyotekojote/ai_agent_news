## ツールハンドラプラン間接参照の削除

ツールハンドラの種類を記録する中間レジストリプランが削除され、具体的なハンドラが直接登録されるようになった。`ToolHandlerKind`、`ToolHandlerSpec`、`ToolRegistryPlan` が廃止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.15)

## OpenAI Developers プラグインの許可リスト追加

`openai-developers@openai-curated` がツール候補の許可リストに追加され、ツール提案を通じて OpenAI Developers プラグインが表示されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.15)

## app-server キューの共有設定読み取り

グローバル app-server リクエストに共有読み取りシリアライゼーションモードが実装された。`skills/list`、`config/read`、`plugin/list` が共有読み取りとしてマークされ、連続した読み取りが排他リクエストの順序を維持しながら同時実行可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.15)

## スキルリスト読み込みの並列化

スキルリストエントリが同時実行数5の制限付きで並列処理されるようになり、マルチルートワークスペースでのコールドスタートレイテンシが削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.15)

## state DB インジェクションとエージェントグラフストアのリバート

スタック全体にわたるオプショナルな state DB プランビングが復元された。ThreadManager 構築からの必須 state DB 依存関係が削除され、インストレーション ID およびセッション/スレッド ID の変更は維持された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.15)

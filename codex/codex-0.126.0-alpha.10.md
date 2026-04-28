## ヒンティング修正 2

MultiAgentV2 コンテキストヒントの問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/19961)

## ヒンティング修正 3

MultiAgentV2 コンテキストヒントの追加修正が行われた。

[参考リンク](https://github.com/openai/codex/pull/19963)

## メモリ Phase 2 入力順序の安定化

Phase 2 メモリ選択ランキングが安定した昇順 `thread_id` 順序で返されるようになった。使用回数、最近使用時刻、ソース更新タイムスタンプ、スレッド ID によるランキングロジックは維持されつつ、出力順序が決定論的になり、トークン消費とワークスペース差分ノイズが削減された。ドキュメントもファイル位置ではなくメタデータとワークスペース差分を最新性シグナルとして使用するよう更新された。

[参考リンク](https://github.com/openai/codex/pull/19967)

## ユーザーターンからのメモリトリガーとクールダウン

メモリのスタートアップトリガーがスレッドライフサイクルイベント（作成、ロード、フォーク）から `thread/sendInput` の非空ターンに移動された。グローバル Phase 2 統合に 6 時間のクールダウンが追加された。デフォルトのメモリスタートアップが 10 日間で最大 2 回のロールアウト、ロールアウト間の最小アイドル時間 6 時間に制限された。

[参考リンク](https://github.com/openai/codex/pull/19970)

## AgentIdentity AuthAPI ベース URL の設定

環境変数 `CODEX_AGENT_IDENTITY_AUTHAPI_BASE_URL` による AuthAPI エンドポイントの設定サポートが追加された。これにより、ローカルおよびステージング環境が内部 URL をハードコードせずに異なる認証プロバイダをターゲットにできるようになった。本番 URL が未指定時のデフォルトとして維持される。

[参考リンク](https://github.com/openai/codex/pull/19904)

## レート制限が低い場合のメモリスタートアップスキップ

残りの Codex バックエンドクォータが設定閾値を下回った場合にメモリパイプラインの起動を延期するガード機能が実装された。新しい設定 `memories.min_rate_limit_remaining_percent`（デフォルト 25%、範囲 0-100）が追加された。`codex.memory.startup` カウンターに `status=skipped_rate_limit` トラッキングが追加された。

[参考リンク](https://github.com/openai/codex/pull/19990)

## メモリのハウスキーピング 1

メモリ関連のメトリクスが専用ファイルに移動され、コードの整理が行われた。

[参考リンク](https://github.com/openai/codex/pull/19998)

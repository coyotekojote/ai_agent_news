## スポーンエージェントメタデータのデフォルト非表示化

MAv2 CBv9互換性のため、`hide_spawn_agent_metadata`がデフォルトで`true`に設定された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## コンテキストフラグメントの独立クレート化

再利用可能なフラグメント機構が`codex-core`から分離され、新たに`codex-context-fragments`クレートとして抽出された。他のパッケージがコア依存関係全体を取り込まずにこの抽象化に直接依存できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## MAv2 close_agentの自己ターゲット拒否

ワーカーが`close_agent`を自分自身に対して使用することを防ぐガードが追加された。結果を返すよう指示するモデル可視エラーが返される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## スキルのターン入力コントリビューター移行

スキル拡張が`TurnLifecycleContributor`から`TurnInputContributor`に移行され、エグゼキュータスコープのスキルルーティングに必要な環境IDやワーキングディレクトリへのアクセスが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## ゴール進行状況の会計シリアライズ

スレッドごとの進行状況会計パーミットが追加され、複数のツール完了フックが同時実行される際のトークンデルタの二重計上が防止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## Session IDの名前変更

自動リファクタリングにより`Session::conversation_id`が`Session::thread_id`にリネームされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## v1スキル拡張プロンプトインジェクション

候補スキルのリスト化と選択されたメインプロンプトのインジェクションのための権限保持フローが実装された。カタログ展開、プロバイダールーティング、および制限付きスキルレンダリングが含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

## WindowsセットアップヘルパーのUACマニフェスト復元

`asInvoker`実行レベルの最小限のUACマニフェストが復元され、非昇格セットアップリフレッシュ時に昇格が要求されなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0-alpha.5)

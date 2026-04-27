## `/auto-review-denials` リトライ承認フロー

拒否されたアクションを選択してリトライの承認コンテキストを送信できる TUI サーフェスが追加された。

[参考リンク](https://github.com/openai/codex/pull/19058)

## Codex issue digest スキル

メンテナー向けに GitHub イシューダイジェストを生成する再利用可能なスキルが追加された。決定論的な収集とアクティビティメトリクスを備えている。

[参考リンク](https://github.com/openai/codex/pull/19779)

## git ベースのワークスペース diff によるメモリ統合

メモリ Phase 2 が git diff を使用した統合をサポートするようになった。手動編集や拡張にも対応している。

[参考リンク](https://github.com/openai/codex/pull/18982)

## パーミッションプロファイル移行の完了

アプリケーションサーフェス全体でのパーミッションプロファイル実装が完了した。レガシーサンドボックスポリシーの投影が正規ヘルパーに集約され、ストレージは制約付きプロファイルのみを保持するようになった。レガシー exec ポリシーは互換性境界でオンデマンドに導出される。

[参考リンク](https://github.com/openai/codex/compare/rust-v0.126.0-alpha.4...rust-v0.126.0-alpha.6)

## リモートサンドボックス設定のホスト名解決改善

リモートサンドボックス設定のホスト名解決がインラインで行われるようになり、ホスト名ルックアップが遅いシステムでの起動パフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/pull/19739)

## `multi_agent_v2` のスレッドキャップ設定移動

MultiAgentV2 セッションのスレッドキャップがフィーチャー設定に移動され、デフォルト値は 4 に設定された。

[参考リンク](https://github.com/openai/codex/pull/19792)

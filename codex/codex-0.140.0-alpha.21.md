## フィードバックアップロードのサブツリー上限

フィードバックログのアップロードがSQLiteログ集約前に最大8スレッドに制限されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28332)

## 動的ツールの明示的名前空間表現

動的ツールが内部的に明示的な名前空間メタデータを保持するようリファクタリングされた。`thread/start` APIも明示的な名前空間オブジェクトを受け付けるようになった。

[参考リンク](https://github.com/openai/codex/pull/27365)

## ローカルエグゼキューター使用時のオーケストレータースキル非表示

ローカルエグゼキューターを持つスレッドでホストされたスキルカタログの重複が防止されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28333)

## シェルスナップショットの所有権簡素化

スナップショットのライフサイクル管理とファイル所有権パターンがリファクタリングされた。

[参考リンク](https://github.com/openai/codex/pull/27756)

## ターミナルリサイズリフローの安定化

`terminal_resize_reflow`が安定版としてマークされ、非推奨のコードパスが削除された。

[参考リンク](https://github.com/openai/codex/pull/27794)

## exec-serverリレーのキープアライブ復元

rendezvousリレーの両エンドポイントで定期的なWebSocket pingフレームが復元された。

[参考リンク](https://github.com/openai/codex/pull/28286)

## メモリ読み取りメトリクスの簡素化

テレメトリにおける重複したシェルコマンド再構築が排除された。

[参考リンク](https://github.com/openai/codex/pull/28164)

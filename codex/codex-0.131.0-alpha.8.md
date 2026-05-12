## ログイントークンの失効処理

再ログイン成功後に以前保存されたマネージドChatGPTトークンが失効されるようになった。ブラウザログインとデバイスコードログインの両フローに対応し、失効処理が失敗してもログイン自体は成功する。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## ネットワークプロキシ機能（実験的）

パーミッションプロファイルのネットワーク設定とは独立した実験的ネットワークプロキシ機能が追加された。`[features.network_proxy]`テーブルで設定でき、アクティブなパーミッションプロファイルまたはレガシーサンドボックスモードでネットワークアクセスが有効な場合にのみ動作する。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## Python SDKの大幅刷新

Python SDKが全面的にリファクタリングされた。ディストリビューション名が`openai-codex-app-server-sdk`から`openai-codex`に変更された。明示的なランタイム依存関係のピン留め、キュレートされたパブリックAPIサーフェスの定義、`ApprovalMode`列挙型（`auto_review`と`deny_all`オプション）の追加、app-serverテスト用統合ハーネスの実装、Ruffによるフォーマット・リント設定が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## アナリティクスレビューイベント

完了したユーザーレビューおよびガーディアンレビューに対して汎用的な`codex_review_event`行が出力されるようになった。subject、reviewer、trigger、status、resolution、durationが記録され、`shell`と`unified_exec`の承認ソースが区別される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## Windowsフック用コマンドオーバーライド

フック設定に既存の`command`フィールドに加えてオプションの`command_windows`フィールドが追加された。Windowsシステムでのみプラットフォーム固有のオーバーライドが適用される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## リモートコントロールのデーモン統合

`codex remote-control`が新しいapp serverデーモンコマンドを使用するように更新され、ブートストラップと永続化設定の有効化が行われた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

## 承認行フィンガープリントの変更

承認行アナリティクスイベントでパス/行ハッシュのフィンガープリントがアップロードされなくなった。ローカルのパース処理と集計行数は維持される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.8)

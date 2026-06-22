## サンプリング前の環境コンテキスト更新

リモート環境が同一ターン中にスタートアップを完了した際に、モデルに見えるよう環境コンテキストが更新されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29073)

## x-codex-turn-metadata の thread_source 復元

誤って削除された `thread_source` フィールドが復元され、キーが予約された。

[参考リンク](https://github.com/openai/codex/pull/29455)

## 永続ログからのノイズの多いターゲットフィルタリング

高ボリュームの依存関係ログと OpenTelemetry ミラーイベントが SQLite シンクから除外されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29457)

## 画像準備のフラグ削除

Fjord の集中型画像準備が新規および再開履歴に対して無条件で適用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29429)

## プラグイン分析メタデータの集約

プラグインテレメトリのメタデータ構築がローダーヘルパーから PluginsManager に移動された。

[参考リンク](https://github.com/openai/codex/pull/27102)

## TUI プラグイン共有: リモートプラグインカタログセクションのレンダリング

OpenAI Curated、Workspace、Shared セクションがローディング/空/エラー状態とともにレンダリングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/26703)

## リモートサンドボックス拒否のセマンティックレポート

エグゼキューターが実装の詳細を公開せずにサンドボックス拒否をポータブルに報告できるようになった。

[参考リンク](https://github.com/openai/codex/pull/29424)

## metadata フィールドの名称変更

汎用的な metadata フィールドが `internal_chat_message_metadata_passthrough` に強い型付けされたパススルーフィールドに移行された。

[参考リンク](https://github.com/openai/codex/pull/28968)

## Python SDK での HTTP 画像 URL 非推奨化

Python SDK の例でデータ URL が使用されるようになり、HTTP/HTTPS 画像 URL が非推奨となった。

[参考リンク](https://github.com/openai/codex/pull/29464)

## 使用量制限リセットの文言・状態修正

使用量制限の用語が更新され、クレジット引き換え後の古い残高保持の問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/28793)

## Guardian 子セッションの親セッション開始時の生成

親セッションの初期化時に Guardian 子セッションが作成されるようになり、レイテンシが削減された。

[参考リンク](https://github.com/openai/codex/pull/27982)

## 未使用の permissions cwd 配管の削除

パーミッションコンパイル関数から未使用の `_policy_cwd` パラメータが削除された。

[参考リンク](https://github.com/openai/codex/pull/29468)

## 共有認証システムプロキシ契約の追加

ルート認識型の auth/system-proxy 境界が MVP ルーティングポリシーとともに追加された。

[参考リンク](https://github.com/openai/codex/pull/26707)

## メールなし ChatGPT アカウントの許可

アカウントメタデータでメールがオプションとなり、全レイヤーを通じてメールの不在が保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28991)

## ロールアウト予算リマインダーしきい値の設定化

固定間隔の代わりに残りトークンに基づく設定可能なリマインダーしきい値が導入された。

[参考リンク](https://github.com/openai/codex/pull/29423)

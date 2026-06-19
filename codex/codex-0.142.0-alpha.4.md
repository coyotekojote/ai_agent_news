## UUIDv7コンテキストウィンドウIDの追加

コンテキストウィンドウにUUIDv7を使用した安定した不透明な識別子が追加された。

[参考リンク](https://github.com/openai/codex/pull/28953)

## リモートインストール後のプラグイン・ツールキャッシュリフレッシュ

リモートプラグインのインストール後にプラグインおよびツールのキャッシュがリフレッシュされ、インストール済みプラグインがツールカタログに即座に表示されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28951)

## Realtime WebRTCのAVAS固定

リアルタイムアーキテクチャセレクターが削除され、WebRTCがAVAS/v1に固定された。

[参考リンク](https://github.com/openai/codex/pull/28856)

## 履歴記録時のレスポンスアイテムID割り当て

ロールアウトとリジュームをまたいでアイテムIDが永続化されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28814)

## リモートプラグインのキュレートリポジトリ同期スキップ

リモートプラグインがアクティブな場合、レガシーのリポジトリ同期が省略されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29005)

## clock current-timeツールの追加

モデルのツール呼び出しからタイムプロバイダーにアクセスできるclockツールが追加された。

[参考リンク](https://github.com/openai/codex/pull/29011)

## 圧縮置換履歴へのアイテムID割り当て

リモートv2の圧縮置換アイテムにIDが割り当てられるようになった。

[参考リンク](https://github.com/openai/codex/pull/29012)

## 保護リソースのOAuthディスカバリーサポート

プラグインのOAuthディスカバリーが上流のMCP SDKに委譲されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29022)

## リモート環境接続ライフサイクルの実装

リモート環境のバックグラウンド接続起動が実装された（3部構成の1/3）。

[参考リンク](https://github.com/openai/codex/pull/28674)

## スナップショットでの起動中環境追跡

解決中の非ブロッキングな環境スナップショットが可能になった（3部構成の2/3）。

[参考リンク](https://github.com/openai/codex/pull/28683)

## 環境接続タイムアウトの設定

環境のWebSocket接続タイムアウトが設定可能になった（3部構成の3/3）。

[参考リンク](https://github.com/openai/codex/pull/29025)

## ターンごとのマルチエージェントモードの追加

マルチエージェントv2でターンごとの委任モード選択が有効になった。

[参考リンク](https://github.com/openai/codex/pull/28685)

## スレッドレベルのマルチエージェントモードの公開

マルチエージェントモードのスレッド初期化およびライフサイクルAPIが追加された。

[参考リンク](https://github.com/openai/codex/pull/28792)

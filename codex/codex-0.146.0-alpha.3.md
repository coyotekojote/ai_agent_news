## Git Attribution拡張機能の追加

新しいコンテキストコントリビューター`codex-git-attribution`が追加された。ワークスペースのcommit_attribution_enabled設定を解決し、World State経由でコミット/PR帰属指示を配信する。ポリシーキャッシングとエラーハンドリングを含む。アプリサーバー、MCPサーバー、デバッグツールにインストールされた。

[参考リンク](https://github.com/openai/codex/pull/34769)

## JSON直列化オーバーヘッドの削減

アプリサーバーのJSON直列化コストを削減するパフォーマンス最適化が行われた。型付きアプリサーバーリクエストの直列化オーバーヘッドもさらに削減された。

[参考リンク](https://github.com/openai/codex/pull/34761)

## スキルカタログのメタデータ圧力下での保持改善

メタデータスペースが制約されている場合でもスキルカタログエントリが表示されるようになった。エントリ全体を削除する前にまず説明文をドロップする戦略に変更された。切り詰め時の通知レポートも追加された。

[参考リンク](https://github.com/openai/codex/pull/34732)

## リアルタイムV3 APIのBEMチャネルプレフィックス設定

`codexResponseHandoffChannelPrefixes`パラメータが追加され、リアルタイムV3 APIの`[ANALYSIS]`、`[COMMENTARY]`、`[FINAL]`チャネルルーティングプレフィックスをカスタマイズできるようになった。

[参考リンク](https://github.com/openai/codex/pull/34816)

## サンドボックスプロンプトのネットワークアクセス表示修正

サンドボックステンプレートが`{{ network_access }}`プレースホルダーを使用するよう更新され、権限プロンプトがアクティブなネットワークアクセス状態を動的に反映するようになった。

[参考リンク](https://github.com/openai/codex/pull/34811)

## 4KiBを超える行のシンタックスハイライトスキップ

非常に長い行（4KiB超）に対する高コストなシンタックスハイライトがスキップされるようパフォーマンスが修正された。

[参考リンク](https://github.com/openai/codex/pull/34796)

## WebSocketリクエストのリトライ追加

前のレスポンスが欠落しているWebSocketリクエストに対するリトライロジックが追加された。

[参考リンク](https://github.com/openai/codex/pull/34763)

## 統一メンションポップアップのサイズ調整

メンションポップアップのサイズが実際の表示結果に合わせて調整されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34771)

## セッションヘッダーの狭いターミナル幅への対応

セッションヘッダーが狭いターミナルウィンドウからオーバーフローしないようクランプされた。

[参考リンク](https://github.com/openai/codex/pull/34775)

## ターン完了サマリーへの最終エージェントメッセージ追加

ターン完了サマリーに最終エージェントメッセージが含まれるようになった。

[参考リンク](https://github.com/openai/codex/pull/34777)

## TUIターミナルのOSC 8ハイパーリンク統合

ターミナルUIでのハイパーリンクレンダリングが改善され、ラップされたOSC 8ハイパーリンクが統合された。

[参考リンク](https://github.com/openai/codex/pull/34778)

## コンパクション時間のターンプロファイル追跡

ターンプロファイルとアナリティクスに`compaction_ms`が追加された。コンパクションが独自の排他的プロファイルフェーズに分離され、パフォーマンスの可視性が向上した。

[参考リンク](https://github.com/openai/codex/pull/34835)

## `local`名の動的環境の拒否

予約名「local」を使用した動的環境の作成が拒否されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34784)

## インプロセスアプリサーバーシャットダウン前のアナリティクスフラッシュ

アプリサーバーのシャットダウン前にアナリティクスイベントがフラッシュされるようになった。

[参考リンク](https://github.com/openai/codex/pull/34831)

## Responsesリクエスト構築時のクローン削減

APIリクエスト構築時のメモリ割り当てを削減するパフォーマンス最適化が行われた。

[参考リンク](https://github.com/openai/codex/pull/34825)

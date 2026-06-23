## /usage コマンドによる使用量リセットクレジットの表示・引き換え

`/usage` コマンドで獲得した使用量制限リセットクレジットの表示と引き換えが可能になり、確認、リトライ、更新状態がサポートされた。

[参考リンク](https://github.com/openai/codex/pull/28154)

## /plugins のリモートプラグインセクション整理

リモートプラグインが OpenAI Curated、Workspace、Shared with me セクションに整理され、対象ターンで関連プラグインの推薦とインストールが可能になった。

[参考リンク](https://github.com/openai/codex/pull/26703)

## ロールアウトトークンバジェットの設定化

エージェントスレッド間のトークン使用量を追跡する設定可能なロールアウトバジェットが導入され、残りバジェットのリマインダーと枯渇時のターン中止機能が追加された。

[参考リンク](https://github.com/openai/codex/pull/28746)

## マルチエージェント委任モードの設定

アプリサーバークライアントがスレッドおよびターンレベルで無効、明示的リクエストのみ、プロアクティブの3モードでマルチエージェント委任を設定できるようになった。

[参考リンク](https://github.com/openai/codex/pull/28685)

## インデックス付きウェブ検索モード

サーバー承認済みURLへの直接アクセスを制限しつつ、ライブ検索を許可するインデックス付きウェブ検索モードが追加された。

[参考リンク](https://github.com/openai/codex/pull/28489)

## UTC 時刻リマインダーと現在時刻クエリ

スケジュールされた UTC 時刻リマインダーの受信と、クライアント提供のアプリサーバークロックを介した現在時刻のクエリが可能になった。

[参考リンク](https://github.com/openai/codex/pull/28822)

## Linux TUI の suspend/resume 後のレンダリング復元

Ctrl+Z による suspend と fg resume 後の Linux TUI レンダリングが復元された。

[参考リンク](https://github.com/openai/codex/pull/28342)

## exec-server プロセスの一時的な切断耐性

exec-server プロセスと stdio MCP セッションが一時的な切断に耐えるようになり、署名済み URL のリフレッシュとリトライセーフな stdin 書き込みが含まれた。

[参考リンク](https://github.com/openai/codex/pull/28512)

## リモート環境のパス・シェル・サンドボックス保持

リモート環境がエクゼキュータネイティブのパス、シェル、AGENTS.md 検出、サンドボックス動作をOS間で保持するようになった。

[参考リンク](https://github.com/openai/codex/pull/28146)

## プラグイン読み込みのマニフェストフォールバック対応

プラグイン読み込みがルートマーケットプレイスレイアウト、マニフェストフォールバック、複数スキルパス、エラー時のダウンロードメッセージ、即時ツールリフレッシュに対応した。

[参考リンク](https://github.com/openai/codex/pull/28771)

## サブエージェントのターミナルエラー伝達

親エージェントが空の成功応答ではなく、サブエージェントのターミナルエラーを受信するようになった。

[参考リンク](https://github.com/openai/codex/pull/28375)

## goal-first スレッドの永続化復元

goal-first スレッドが thread/list および thread/search で永続化・返却されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28808)

## 起動・セッションレイテンシの削減

DNS 処理の遅延、モデルキャッシュのウォームアップ、パース済みプラグインスキルの再利用、メタデータ読み取りの並列化、冗長なカタログ同期のスキップにより、起動とセッションのレイテンシが削減された。

[参考リンク](https://github.com/openai/codex/pull/28542)

## 永続ログの最適化

WebSocket イベントごとのペイロードログとテレメトリレコードの重複が削除され、永続ログが最適化された。

[参考リンク](https://github.com/openai/codex/pull/29432)

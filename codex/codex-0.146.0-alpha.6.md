## Agent Pluginsマニフェストのサポート

Agent Pluginsマニフェストがサポートされた。プラグインの定義と管理が標準化されたマニフェスト形式で行えるようになった。

[参考リンク](https://github.com/openai/codex/pull/35105)

## コードモードホストへのWebSocketトランスポート追加

コードモードホストにWebSocketトランスポートが追加された。リアルタイム通信のためのWebSocket接続が可能になった。

[参考リンク](https://github.com/openai/codex/pull/35078)

## リモートコードモードホストのapp-serverサポート

app-serverでリモートコードモードホストがサポートされるようになった。リモート環境でのコードモード実行が可能になった。

[参考リンク](https://github.com/openai/codex/pull/35098)

## ホストによるwait_for_environment説明のカスタマイズ

ホストが`wait_for_environment`の説明をカスタマイズできるようになった。環境待機時のユーザー向けメッセージを変更可能になった。

[参考リンク](https://github.com/openai/codex/pull/35106)

## Guardian V2フィーチャーフラグの登録

Guardian V2のフィーチャーフラグが登録された。次世代のGuardianシステムの段階的ロールアウトが可能になった。

[参考リンク](https://github.com/openai/codex/pull/35049)

## update_planツールの無効化設定

`update_plan`ツールを無効化できる設定が追加された。

[参考リンク](https://github.com/openai/codex/pull/35054)

## exec-serverのWebSocket通信のプロキシ対応

exec-serverのWebSocket通信が設定済みプロキシを経由するようになった。

[参考リンク](https://github.com/openai/codex/pull/35056)

## exec-serverのHTTPとreqwest型の分離

exec-serverのHTTPレイヤーがreqwest型から分離され、柔軟なHTTPクライアント実装が可能になった。

[参考リンク](https://github.com/openai/codex/pull/35059)

## ツール検索における遅延ソースの重複排除

ツール検索で遅延ソースが重複して表示される問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/35065)

## ワールドステートでの遅延ツールネームスペース追跡

遅延ツールのネームスペースがワールドステートで追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35063)

## Bazelテスト設定のプラットフォーム固有データ修正

プラットフォーム固有データに関するBazelテスト設定が修正された。

[参考リンク](https://github.com/openai/codex/pull/35067)

## アプリ/読み取りリクエスト時間の追跡

アプリおよび読み取りリクエストの所要時間が追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35048)

## Windowsサンドボックスのプロキシ設定保持

Guardianセッション内でWindowsサンドボックスのプロキシ設定が保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35036)

## 環境レジストリリクエストの共有HTTPクライアント経由化

環境レジストリリクエストが共有HTTPクライアントを経由するようになった。

[参考リンク](https://github.com/openai/codex/pull/35034)

## Browser Use要件のapp-server公開

Browser Useの要件がapp-serverを通じて公開されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35033)

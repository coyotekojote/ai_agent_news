## PathUri のホストネイティブパス変換の明確化

`PathUri::from_path` が `PathUri::from_host_native_path` にリネームされ、意味が明確化された。

[参考リンク](https://github.com/openai/codex/pull/29501)

## リモートプラグインカタログフローのテスト追加

ワークスペース、共有、ローカルソース、タブ永続化、重複排除、マーケットプレイスエラーハンドリングのリモートプラグインカタログの回帰テストが追加された。

[参考リンク](https://github.com/openai/codex/pull/26704)

## アプリサーバーインジェストでのリモート画像拒否

ターンハンドラーで HTTP(S) 画像 URL がバリデーションとテキストフォールバック付きで拒否されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29419)

## 期限切れ Bedrock 認証情報エラーの改善

期限切れの AWS 認証情報に対するプロバイダー固有のエラーマッピングが追加され、対処方法のガイダンスが提供されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28992)

## フォーマッターの成功時出力の静音化

フォーマッターの出力がバッファリングされ、失敗時のみ表示されるようになり、`just fmt` 実行時のノイズが削減された。

[参考リンク](https://github.com/openai/codex/pull/29467)

## macOS システムプロキシリゾルバーの追加

SystemConfiguration と CFNetwork を使用した macOS システムプロキシ解決が PAC/WPAD サポート付きで実装された。

[参考リンク](https://github.com/openai/codex/pull/26709)

## Code Mode のモデルメタデータ不足時の警告

Code Mode に必要なモデルメタデータが欠けている場合に警告が表示されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29490)

## リモート stdio MCP サーバーの外部絶対パス cwd 受け入れ

リモート MCP サーバーがホストと異なるパス規約を使用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/29493)

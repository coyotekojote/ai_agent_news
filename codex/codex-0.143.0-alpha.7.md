## PathUri の字句的包含判定の追加

PathUri に字句的包含判定が追加され、URI オーソリティが完全なパスセグメントで比較されることで類似パスの区別が可能になった。

[参考リンク](https://github.com/openai/codex/pull/29614)

## レジューム時のロールアウト履歴共有

レジューム時のロールアウト履歴が `Arc<Vec<RolloutItem>>` として保存されるようになり、ディープクローンが不要となりコールドレジュームのレイテンシが約9-10%削減された。

[参考リンク](https://github.com/openai/codex/pull/28426)

## rmcp の 1.8.0 へのアップデート

`rmcp`/`rmcp-macros` が 1.7.0 から 1.8.0 にアップデートされ、新しい `peer_info` 戻り値型への対応と、Rust のトレイト再帰オーバーフローを防ぐための OAuth ステータスディスカバリのボックス化が行われた。

[参考リンク](https://github.com/openai/codex/pull/29634)

## 脆弱な Hono と fast-uri 依存関係のアップデート

`hono` が 4.12.25 に、`fast-uri` が 3.1.1 にピン留めされ、fast-uri のパーセントエンコードされたパストラバーサルに関するセキュリティ脆弱性が修正された。

[参考リンク](https://github.com/openai/codex/pull/29650)

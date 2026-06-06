## Opペイロードのserde最適化

サブミッション側の`Op`ペイロードおよび関連型からserdeアノテーションが削除された。シリアライゼーションは外部API用にのみ保持され、複雑さが軽減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## ゴールエラー時の自動ブロック

ターンが非リトライ可能エラーまたはリトライ回数超過で終了した場合、アクティブなゴールが自動的にブロックされるようになった。HTTP 400などの永続的なエラーでの繰り返し失敗が防止される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## レガシーリモートプラグイン同期の削除

`/plugins/list`を呼び出していたレガシーリモートプラグイン同期パスが削除された。`sync_plugins_from_remote` APIは廃止され、現行のリモートカタログフローは維持される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## v2パーソナルアクセストークンのサポート

`codex login --with-access-token`および`CODEX_ACCESS_TOKEN`環境変数によるv2パーソナルアクセストークン（PAT）サポートが導入された。AuthAPIを通じたメタデータハイドレーションも含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## Responses Liteのスタンドアロンツール対応

Responses Liteがウェブ検索と画像生成にホステッドエグゼキューターではなくスタンドアロンツールを使用するよう構成された。適切なトランスポートヘッダー（`X-OpenAI-Internal-Codex-Responses-Lite: true`）が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## マネージド権限プロファイルのアローリスト

マネージド権限プロファイルのアローリストがマージ可能なマップとして実装された。構成レイヤー間でのエンタープライズセキュリティ境界が実現され、リストにないプロファイルは明示的に拒否される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

## UIとテストの改善

TUIでのターミナルビジュアライゼーション指示のフィーチャーゲートが追加された（デフォルト無効）。スキルロード警告の重複排除が実装された。ベンチマークスモークテストが標準の`just test`コマンドから除外された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.6)

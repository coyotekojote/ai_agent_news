## システムプロキシ（PAC）機能の設定サーフェス追加

`respect_system_proxy` フィーチャーフラグが追加され、ネイティブクライアントのシステムプロキシ/PAC対応の基盤が整備された（デフォルト無効）。

[参考リンク](https://github.com/openai/codex/pull/26706)

## リモートプラグインカタログの認証ゲート

リモートグローバルプラグインカタログが認証済みユーザーかつ `remote_plugin` が有効なユーザーのみに制限されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28625)

## オブジェクト値プラグインMCPマニフェストのサポート

プラグインマニフェスト解析が拡張され、`plugin.json` 内でMCPサーバーを直接オブジェクトとして指定できるようになった。

[参考リンク](https://github.com/openai/codex/pull/28580)

## 画像生成結果の永続化改善

ステータスが `generating` のままの画像生成アイテムが完全なPNGデータとともに永続化されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28656)

## exec-serverセッションの切断後再接続

exec-serverのプロセスおよびMCPレイヤー下での再接続が実装され、切断後にハンドルの保持と欠落出力の回復が可能になった。

[参考リンク](https://github.com/openai/codex/pull/28512)

## 冗長なTurnContextおよびPromptフィールドの削除

重複してキャッシュされていたフィールドが削除され、値がconfigまたはmodel_infoから直接取得されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28638)

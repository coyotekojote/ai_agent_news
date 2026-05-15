## レイヤードprofile-v2設定ファイルの追加

レイヤード`--profile-v2`設定ファイルが追加され、プロファイル設定の柔軟な管理が可能になった。profile-v2使用時にレガシー`[profiles]`が拒否されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

## プラグインマーケットプレイスCLIコマンドの追加

プラグインマーケットプレイスのCLIコマンドが追加され、プラグインの検索・インストールがCLIから可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

## 明示的MCP OAuthクライアントIDのサポート

明示的なMCP OAuthクライアントIDがサポートされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

## リモートコントロールのランタイム切り替え

リモートコントロールの有効化/無効化がfeatureフラグではなくランタイムで行えるようになり、リモートコントロールデーモンのUXが改善された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

## ToolExecutorの非同期トレイト化

`ToolExecutor`がasyncトレイトに変更され、ツール実行の柔軟性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

## バグ修正

TUIでネットワーク承認履歴がターゲットごとにレンダリングされるようになった。Gitメタデータ読み取り時にfsmonitor設定が無視されるようになった。PowerShellのstop-parsing形式が未サポートとして扱われるようになった。起動NUXインプレッションが起動成功まで遅延されるようになった。state DBがオープンできない場合にapp-serverの起動がブロックされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.19)

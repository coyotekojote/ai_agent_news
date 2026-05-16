## サンドボックスのテレメトリタグ付け改善

サンドボックスのテレメトリタグ付けがレガシーの`SandboxPolicy`から`PermissionProfile`ベースのアプローチに移行された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.22)

## スレッドAPIからの権限プロファイル応答削除

app-serverのスレッドライフサイクルAPIレスポンスから`permissionProfile`フィールドが削除された。クライアントはフルプロファイル値ではなくアクティブなプロファイルIDのみをラウンドトリップするようになり、レスポンス由来のプロファイルによる意図しない権限拡大が防止された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.22)

## リモートコントロールAPIの改善

app-serverのリモートコントロールAPIに`server-name`パラメータが追加され、新しい`remoteControl/status/read`エンドポイントが導入された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.22)

## macOS署名済みプロモーションのDMGステージング無効化

署名済みmacOSプロモーションパスでDMGステージングが無効化され、不要な公証要件を削除することでリリースワークフローが合理化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.22)

## バグ修正

SQLiteメタデータの書き込み失敗がノンブロッキングになり、明示的なgit専用メタデータ更新のハード失敗は維持された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.22)

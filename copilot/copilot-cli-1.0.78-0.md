## /permissionsコマンドの追加

承認モードを切り替えるための新しい`/permissions`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## ACPモードのセッション終了対応

ACPモードにおいて、`closeSession`リクエストによるセッションの終了がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## サンドボックスのツールチェーンキャッシュアクセス

新しいサンドボックス設定`allowDevToolCaches`（デフォルト有効）が追加され、サンドボックス化されたビルドがツールチェーンキャッシュ、レジストリ、インストールにアクセスできるようになった。追加設定なしでビルドが動作する。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## GitHub MCP明示的設定の尊重

明示的なGitHub MCPのツールセット/ツール設定が尊重されるようになり、オプトインしているユーザーに対して`gh` CLIの使用を誘導しないようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## settings.jsonの未知キー警告

起動時にユーザーの`settings.json`内の未知のトップレベルキーに対して警告が表示されるようになった（従来はサイレントに無視されていた）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## --modelフラグのシェル補完

`--model`フラグのシェル補完で「auto」およびサポートされているモデル名が候補として表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## セッショントランスクリプトの段階的レンダリング

長いセッショントランスクリプトが段階的にレンダリングされるようになり、スクロールのレスポンスが向上した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## セッション再開パフォーマンスの大幅改善

セッション再開のパフォーマンスが劇的に改善された。230MBのトランスクリプト（74kイベント）が1秒未満でロードされるようになった（従来は約10秒）。ピークメモリ使用量も約25%に削減された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## バグ修正

Ctrl+Qがハイライトされたテキスト中のスキル補完を正しくキューに入れるように修正された。セッション切り替え時にMCPサーバーの再起動やフック状態の再構築が行われなくなった。OAuth認証後に遅延MCPツールがリフレッシュされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

## /allow-allの安全判定モデル設定の削除

`/allow-all`の自動安全判定モデルがユーザー設定不可となり、モデル選択が自動化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-0)

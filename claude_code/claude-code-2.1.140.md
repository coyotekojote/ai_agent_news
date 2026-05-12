## Agent toolのsubagent_typeマッチング改善

Agent toolの`subagent_type`マッチングが大文字・小文字やセパレータを区別しないようになった（例: `"Code Reviewer"`が`code-reviewer`に解決される）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントカラーパレットの更新

エージェントのカラーパレットが更新された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

`/goal`が`disableAllHooks`や`allowManagedHooksOnly`設定時にサイレントにハングする問題が修正され、インジケーターが解決しない代わりに明確なメッセージが表示されるようになった。シンボリックリンクされた設定ファイルによる`ConfigChange`フックの誤発火が修正された。`claude --bg`がバックグラウンドサービスのアイドル終了直前に「connection dropped mid-request」で失敗する問題が修正された。エンタープライズエンドポイントセキュリティ環境でのバックグラウンドサービス起動の待機時間が延長された。リモートマネージド設定が401エラー時にトークンを強制リフレッシュしてリトライするようになった。マネージド`extraKnownMarketplaces`の自動更新ポリシーが`known_marketplaces.json`に永続化されない問題が修正された。`/loop`が完了通知済みのバックグラウンドタスクに対して冗長なポーリングをスケジュールする問題が修正された。Windowsで存在しない実行ファイル（例: `gh`）による同期的な`where.exe`再起動がイベントループを停止させる問題が修正された。`Read`ツールの`offset`パラメータが空白パディングや`+`プレフィックス付き文字列の場合にバリデーションが失敗する問題が修正された。ターミナルのフォーカスが外れた際にネイティブターミナルカーソルが入力キャレットに留まらない問題が修正された。プラグインの`plugin.json`で設定されたキーにより、デフォルトコンポーネントフォルダ（例: `commands/`）がサイレントに無視される場合に警告が表示されるようになった（`/doctor`、`claude plugin list`、`/plugin`で確認可能）。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.140)

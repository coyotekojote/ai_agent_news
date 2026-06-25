## /rewindの/clearサポート

`/rewind`が`/clear`実行前の会話ポイントからの再開をサポートするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクロール位置のジャンプ修正

ストリーミングレスポンス中に以前の出力を読んでいる際にスクロール位置が底にジャンプする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントの停止修正

停止されたバックグラウンドエージェントが復活する問題が修正された。タスクパネルからのエージェント停止が恒久的になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /voiceのポリシーメッセージ改善

organizationのポリシーで無効化されている場合に`/voice`が汎用的な「not available」メッセージではなく制限を説明するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /loginのURL修正

Windows Terminalで行をまたいで折り返す場合に`/login` URLが切り詰められて開かれる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サンドボックスネットワーク権限の改善

「Yes」で許可したホストがセッション残りで記憶されるようになり、接続ごとに再プロンプトされなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPサーバー信頼性の改善

能力発見（`tools/list`、`prompts/list`、`resources/list`）が一時的なネットワークエラーに対してショートバックオフで再試行するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP OAuthの改善

ディスカバリーとトークンリクエストが一時的なネットワークエラー後に1回再試行するようになった。ヘッドレス環境ではブラウザポップアップをスキップしてURL貼り付けプロンプトに直接遷移する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPエラーメッセージの改善

HTTP 404エラーがURLを表示しMCP設定を案内するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CPU使用量の削減

テキスト更新を100msにまとめることでストリーミングレスポンス中のCPU使用量が約37%削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長時間セッションのメモリ改善

ターミナル出力キャッシュからの長時間セッションのメモリ増加が削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 管理設定の改善

`forceRemoteSettingsRefresh`がMDMまたはファイルポリシー経由で設定された場合に有効になり、フェッチが`Cache-Control: no-cache`を送信してプロキシが古いレスポンスを返すことを防ぐようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## その他の修正

Ghosttyのssh/tmux上でのCmd+clickリンク、`claude agents`のスラッシュコマンド送信、エージェントビューのファイルシステムパス表示、カンマ区切りマッチャーのフック、`/permissions`の承認永続化、エージェントパネルのスクロール、ウェルカムスプラッシュアートのオーバーフロー、vimモードの検索ヒントなど多数の修正が行われた。

[参考リンク](https://code.claude.com/docs/en/changelog)

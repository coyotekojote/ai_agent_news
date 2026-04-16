## `/tui` コマンドとフリッカーフリーレンダリング

`/tui` コマンドおよび `tui` 設定が追加された。`/tui fullscreen` を実行すると、同一会話内でフリッカーフリーレンダリングに切り替えられる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プッシュ通知ツール

Remote Control と「Push when Claude decides」設定を有効にすると、Claude がモバイルプッシュ通知を送信できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `Ctrl+O` の動作変更とフォーカスビュー

`Ctrl+O` は通常表示と詳細トランスクリプトの切り替え専用となり、フォーカスビューは新しい `/focus` コマンドで個別に切り替える仕様に変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/plugin` の改善

Installed タブで注意が必要なアイテムとお気に入りが上位に表示され、無効なアイテムは折りたたまれるようになった。`f` キーでお気に入り登録が可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/doctor` の改善

MCP サーバーが複数の設定スコープで異なるエンドポイントとして定義されている場合に警告が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション再開時のスケジュールタスク復元

`--resume`/`--continue` で未期限のスケジュールタスクが復元されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Control での追加コマンド対応

`/context`、`/exit`、`/reload-plugins` が Remote Control（モバイル／ウェブ）クライアントから実行可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Write ツールの IDE 差分フィードバック

IDE の差分ビューで提案内容をユーザーが編集してから受け入れた場合、Write ツールがモデルにその旨を通知するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP ツールのハング修正

SSE/HTTP トランスポートでサーバー接続が応答中に切断された際に MCP ツール呼び出しが無期限にハングする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 非ストリーミングフォールバックリトライの修正

API に到達できない場合に非ストリーミングフォールバックリトライが数分間ハングする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## その他の改善・修正

- フルスクリーンモードでの会話自動スクロールを無効にする `autoScrollEnabled` 設定が追加された
- `Ctrl+G` 外部エディタに Claude の最後の応答をコメント付きコンテキストとして表示するオプションが追加された
- Bash ツールがドキュメント記載の最大タイムアウトを超える値を受け付けないよう制限された
- SDK/ヘッドレスセッションが分散トレースリンクのため環境変数 `TRACEPARENT`/`TRACESTATE` を読み取るようになった
- テレメトリ無効ユーザー（Bedrock、Vertex、Foundry）でもセッション要約が有効になった
- フルスクリーンでツール実行中にテキスト選択すると CPU 使用率が高くなる問題が修正された
- 複数の Plugin、Skills、Remote Control 関連の不具合が修正された

[参考リンク](https://code.claude.com/docs/en/changelog)

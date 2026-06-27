## マウスクリック無効化設定の追加

フルスクリーンモードでマウスクリック/ドラッグ/ホバーを無効化し、ホイールスクロールは維持する`CLAUDE_CODE_DISABLE_MOUSE_CLICKS`環境変数が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ハイフン付き識別子のフックマッチャー修正

ハイフン付き識別子（例: `code-reviewer`、`mcp__brave-search`）のフックマッチャーが誤って部分文字列マッチしていた問題が修正され、完全一致するようになった。ハイフン付きMCPサーバーの全ツールにマッチさせるには`mcp__brave-search__.*`を使用する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## macOS音声ディクテーションの無音キャプチャ修正

macOSでデフォルト入力デバイスが変更された後、長時間実行セッションで音声ディクテーションが無音をキャプチャする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スペースなし言語の音声ディクテーション自動送信修正

日本語、中国語、タイ語などスペースなしで記述される言語で音声ディクテーションの自動送信が発火しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 外部プラグインのインストール同意要求修正

プロジェクトの`.claude/settings.json`のみで有効化された外部プラグインが、すべてのローダーパスで明示的なインストール同意を要求しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /pluginの有効化/無効化の修正

プラグインの`plugin.json`の`name`がマーケットプレイスエントリ名と異なる場合に`/plugin`の有効化/無効化が動作しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドジョブの消失・データ損失修正

新しいバージョンのClaude Codeで書き込まれた際にバックグラウンドジョブが`claude agents`から消えたりデータが失われたりする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## クラッシュしたバックグラウンドタスクの再表示修正

クラッシュしたバックグラウンドタスクを再度開く際に、再起動の代わりに最大5秒間空白画面が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェントデーモンの到達不能修正

コントロールソケットの起動に失敗した場合にバックグラウンドエージェントデーモンが到達不能のまま実行され、再起動をブロックする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Linuxの音声モード改善

Linuxの音声モードで、SoXがインストール済みだがオーディオキャプチャデバイスが存在しない場合に「マイクなし」と「SoX未インストール」を区別するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsの完了リスト表示改善

`claude agents`の完了リストが利用可能な縦方向のスペースを埋めるようになった。短いターミナルではヘッダーがコンパクトになり、ライブセッションが見えるように維持される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートセッション起動の改善

コンテナ起動中にプロビジョニングチェックリストが表示されるようになり、リモートセッションの起動体験が改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

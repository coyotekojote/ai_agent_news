## MCP サーバー障害警告の改善

MCP サーバーの障害警告で、名前にスペースを含むサーバーに対して実行可能な `/mcp show` コマンドが提案されるようになった。また、接続エラーの診断に役立つ stderr 出力が含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

## -C フラグの追加

`git -C` と同様に、起動前に作業ディレクトリを変更する `-C` フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

## 終了メッセージのセッション ID 表示

終了メッセージの再開コマンドで、自動生成名の代わりにセッション ID が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

## リモートセッションエクスポートの拡張

リモートセッションのエクスポートが GitHub 以外のリポジトリおよびリポジトリなしのディレクトリをサポートするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

## ラバーダックエージェントの追加

GPT セッション向けのラバーダックエージェントが追加された。Claude を利用しており、`/experimental` から利用可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

## バグ修正

- 操作キャンセル後にセッションが誤って「使用中」の警告を表示する問題が修正された
- リクエストキャンセル後に Enter キーが永続的にスタックする問題が修正された
- ユーザーメッセージがなく、再開するセッションもない場合に終了サマリーが抑制されるようになった
- Windows CLI のアップデートで展開時に ENOENT エラーが発生する問題が修正された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.42)

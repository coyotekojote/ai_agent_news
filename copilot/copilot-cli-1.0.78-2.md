## スプリットビューサイドバーの閉じる確認メッセージの改善

スプリットビューのサイドバーを閉じる際の確認メッセージが「x again to close」（最後のセッションの場合は「x again to exit CLI」）に更新され、2回目の押下が必要であることがより明確になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-2)

## 拡張機能スラッシュコマンドの重複実行修正

複数の拡張機能がロードされている場合に、スラッシュコマンドのハンドラーが1回の呼び出しで複数回実行される問題が修正され、正確に1回だけ実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-2)

## インライン画像のタイムラインスクロール後の表示修正

タイムラインスクロール後にインライン画像の最初の行が繰り返し表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-2)

## パイプ入力時のsessionEndフックの動作修正

パイプされたstdin入力を受け取る実行において、`sessionEnd`フックの動作が`-p`フラグの動作と一致するように修正された。シャットダウン時に1回発火するのではなく、完了したエージェントターンごとに1回、`reason`を`complete`（失敗時は`error`）として発火するようになった。ターン完了前に終了したパイプ実行ではフックが発火しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78-2)

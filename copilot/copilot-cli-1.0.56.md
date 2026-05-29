## Free・Studentユーザーのモデル選択拡張

Free・StudentユーザーがモデルピッカーでAuto以外のモデルを選択可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## Diffビューの刷新

Diffビューが連続スクロール、スティッキーヘッダー、ターミナル全幅表示、テーマ対応カラーで再設計された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## モデルピッカーの改善

モデルピッカーが料金プランごとの正確なコンテキストウィンドウサイズを表示するようになった。コンテキストウィンドウのティア選択がセッションイベントやresume時に永続的に保持されるようになった。推論エフォートピッカーがモデル能力に応じてサポートされていないオプションを非表示にするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## MCP・ツールの改善

MCPツールがテキストコンテンツと構造化ペイロードの両方を表示するようになり、適切に重複排除される。GitHub MCPサーバーがgh CLI利用可能時に冗長なツールを省略し、トークン使用量を削減するようになった。web_fetchツールがHTTPコンテンツネゴシエーションによりMarkdownコンテンツを優先するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## 設定・構成の改善

`builtInAgents.rubberDuck`設定によるラバーダックエージェントの設定が可能になった。設定ファイルがアトミックに書き込まれ、複数CLIプロセスの同時実行時のデータ損失が防止されるようになった。tmuxでKittyキーボードプロトコルが利用不可の場合も拡張キーレポートが正しく動作するようになった。BYOKプロバイダー設定がACPセッションに正しく適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## UI改善

ThemePickerのサイドバイサイドレイアウトが120カラムターミナルで折り返しなしに収まるようになった。コードレビューエージェントが固定デフォルトではなく現在のセッションモデルを使用するようになった。リモートセッションURLがリポジトリのowner/nameを正しく参照するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## バグ修正

`/context`の小トークン凡例フォーマットと空きスペースグリッドの丸め、`/env`出力のファイルパス表示、推論テキストの表示位置、アシスタント応答の単語孤立行、タブ文字貼り付け後のカーソル位置、信頼フォルダ確認メッセージの権限永続性に関する説明などが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.56)

## 課金プランによるモデル制限

FreeおよびStudentプランのトークンベース課金ユーザーがAutoモデル選択のみに制限されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## Claude Opus 4.8対応

Claude Opus 4.8モデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## 推論トークンの表示

セッションのトークン使用量サマリーに推論トークン数が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## カスタムエージェント・スキルの再帰検出

サブディレクトリ内のカスタムエージェントとスキルが再帰的に検出されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## /autopilotコマンドの追加

オートパイロットフォーカスを維持するための`/autopilot`コマンドが追加された。`/goal`がエイリアスとして利用可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## MCP設定画面の改善

MCP設定が専用画面で開くようになり、スクロール可能なリストで表示されるようになった。MCPトークン使用量がサーバーごとに表示される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## フック進捗のストリーミング表示

長時間実行フックからのリアルタイムステータスがストリーミング表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## リモートセッション管理の改善

セッションピッカーからリモートセッションを直接削除できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## セルベースターミナルレンダラーのデフォルト有効化

セルベースのターミナルレンダラーが全ユーザーに対してデフォルトで有効化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## 拡張機能・プラグインの改善

拡張機能ログファイルが拡張機能ごとに個別にキャプチャされるようになった。プロジェクト拡張機能がgitリポジトリ以外のフォルダベースワークスペースでも検出されるようになった。プラグインディレクトリがスキル検索順序で優先されるようになった。`permissions.disableBypassPermissionsMode`設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## バグ修正

信頼されていないフォルダでの起動時のスピナーハング、ゼロサイズCAPI課金バッチのセッション再開、ネイティブバイナリクラッシュ時のJavaScriptフォールバック、キャンバスツールのスキーマ検証、WindowsでのCJK・Unicodeクリップボードコピー、Waylandクリップボード貼り付け、PowerShell 7のMicrosoft Storeインストール検出、設定移行時のレガシースネークケースキー保持などが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55)

## MCPツール検索のデフォルト有効化

MCPツールがサポートされている場合にデフォルトでツール検索を使用するようになり、ツールの発見性が向上した。

[参考リンク](https://github.com/openai/codex/pull/29486)

## macOSシステムプロキシサポート

macOS認証クライアントが`respect_system_proxy`設定を通じてシステムプロキシ、PAC、WPAD設定を使用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/26709)

## プラグインのダークモードロゴ

プラグインがローカルマニフェストおよびリモートカタログを通じて専用のダークモードロゴを提供できるようになった。

[参考リンク](https://github.com/openai/codex/pull/29488)

## セーフティバッファリングUIの強化

アプリがサーバー提供の可視性およびfaster-modelメタデータを使用して、より豊富なセーフティバッファリングUIを表示できるようになった。

[参考リンク](https://github.com/openai/codex/pull/29473)

## プラグインカタログランキング

リモートプラグインカタログがキュレーションされた注目プラグインランキングを返すようになった。

[参考リンク](https://github.com/openai/codex/pull/29485)

## Amazon Bedrockクレデンシャルエラーの改善

期限切れのAmazon Bedrockクレデンシャルが汎用的な認可エラーではなく、対処可能なリカバリガイダンスを表示するようになった。

[参考リンク](https://github.com/openai/codex/pull/28992)

## リモートMCPサーバーのパス対応

リモートstdio MCPサーバーがリモートプラットフォームパス形式の絶対ワーキングディレクトリを受け入れるようになった。

[参考リンク](https://github.com/openai/codex/pull/29493)

## リモート画像入力のバリデーション改善

リモートHTTP(S)画像入力がモデルに可視な明確なバリデーションエラーを返すようになった。インラインデータURLとローカル画像は引き続きサポートされる。

[参考リンク](https://github.com/openai/codex/pull/29417)

## PowerShell ASTセーフティ

セーフティ分類器が検査できない実行可能なAST領域を含むPowerShellコマンドが承認を要求するようになった。

[参考リンク](https://github.com/openai/codex/pull/24092)

## Code Modeの警告

選択されたモデルに必要なメタデータが不足している場合にCode Modeが警告を表示するようになった。

[参考リンク](https://github.com/openai/codex/pull/29490)

## 依存関係の更新

バンドルされたOpenSSLとesbuildがパッチリリースに更新された。

[参考リンク](https://github.com/openai/codex/pull/29487)

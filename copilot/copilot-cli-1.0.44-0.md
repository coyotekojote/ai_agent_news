## ラバーダックサブエージェントのモデル表示

タイムライン表示でラバーダックサブエージェントの解決済みモデルが表示されるようになった（例：`Rubber-duck(claude-opus-4.7)`）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## Free ユーザーのクォータ表示修正

Free ティアユーザーのクォータ表示が常に100%消費と表示されていた問題が修正され、残りの使用量が正確に反映されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## オートパイロットモードのツール権限永続化

オートパイロットモードで付与されたツール権限が `/clear` コマンド後も保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## モデル切り替え時のエフォートレベル修正

`/model` ピッカーでモデルを切り替えた際に、エフォートレベル設定が正しく適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## 権限プロンプト中の Ctrl+C ハング修正

権限プロンプトの入力待ち中に Ctrl+C を押すと CLI がフリーズする問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## スラッシュコマンドピッカーのプロジェクト情報表示

検索結果が一致しない場合でもスラッシュコマンドピッカーにプロジェクト情報が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

## settings.json の無効な URL 処理改善

settings.json 内の無効な URL が CLI 起動の失敗を引き起こさなくなり、警告付きでスキップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44-0)

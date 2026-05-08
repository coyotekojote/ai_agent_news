## /add-dir のパス補完修正

`/add-dir` でのパス補完がちらついたり `@` や `#` ピッカーに傍受されたりする問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## 入力途中のスラッシュコマンドと複数スキル呼び出し

スラッシュコマンドが入力途中でも使用可能になり、1 つのメッセージで複数のスキルを呼び出せるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## userPromptSubmitted フックのダイレクトハンドリング

`userPromptSubmitted` フックがリクエストを直接処理できるようになり、LLM をバイパスしてモデルコールなしでレスポンスを返せるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## マルチアカウントユーザー向けの高速化

`/user list` および `/user switch` がマルチアカウントユーザー向けに高速化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## プレリリースビルドの更新オプション

`copilot update` および `/update` コマンドにオプションの `prerelease` パラメータが追加され、最新のプレリリースビルドを取得できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## ! プレフィックスのシェルコマンド修正

異なるシェル設定において `!` プレフィックスのシェルコマンドが正しく動作しない問題が修正された。シェルエイリアスや rc ファイルの設定も `!` コマンドで動作するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## Free ユーザーの使用量表示修正

Free ユーザーの使用量表示が常に 100% 使用済みと表示される代わりに、残りの使用量が正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## オートパイロットモードのツール権限修正

オートパイロットモードで付与されたツール権限が `/clear` 後に保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## モデルピッカーでの effort レベル修正

`/model` ピッカーでモデルを切り替えた際に effort レベルが正しく適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## パーミッションプロンプト中の Ctrl+C 修正

パーミッションプロンプトが表示されている間に Ctrl+C を押すと CLI がハングする問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## スラッシュコマンドピッカーのプロジェクト情報修正

結果がマッチしない場合にスラッシュコマンドピッカーでプロジェクト情報が表示されたままになるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## settings.json の無効な URL 修正

settings.json の無効な URL エントリが CLI 起動時にクラッシュを引き起こす代わりに警告付きでスキップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

## タイムラインのモデル表示改善

タイムラインにラバーダックサブエージェントの解決されたモデルが表示されるようになった（例：`Rubber-duck(claude-opus-4.7)`）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.44)

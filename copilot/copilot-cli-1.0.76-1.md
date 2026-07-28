## ボイスモードのメディア制御

ボイスモードで録音前に再生中のメディアが一時停止され、録音後に再開されるようになった。macOSおよびWindowsで対応している。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## AIクレジット制限予測コマンドの追加

`/limits predict`コマンドが追加され、類似セッションに基づいたAIクレジット制限の推奨値が提示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## カスタムステータスラインの定期リフレッシュ

カスタムステータスラインコマンドに対して、設定可能な定期リフレッシュが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## スケジュールプロンプトカウンターの表示

フッターにアクティブなスケジュールプロンプトの数が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## web_fetchのプロキシ対応強化

web_fetchが設定済みのサンドボックスプロキシを経由するようになった。`network.allowOutbound`が無効の場合は外部通信が拒否される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## サブエージェント委任の改善

小規模タスクや並列操作におけるサブエージェントへの委任が強化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## ターン中の`/model`変更のキュー処理

ターン中に`/model`で変更を行った場合、現在のレスポンス完了後にキューイングされて適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## キューメッセージ表示の修正

キューメッセージリストに空行や水増しされたメッセージ数が表示される問題が修正された。Ctrl+Cで最新のキューメッセージを削除できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

## マウス設定の即座反映

マウス設定の変更が`/settings mouse`や設定ダイアログからセッション中に即座に反映されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-1)

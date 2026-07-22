## 初回起動時のサンドボックスオプトインスプラッシュ追加

初回起動時にデフォルトサンドボックスへのオプトインを促すスプラッシュ画面が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## Gemini 3.6 Flashモデルのサポート

Gemini 3.6 Flashモデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## セッション多重化の改善

セッションダイアログが多重化されたセッション間で転送されなくなった。セッション切り替え時にピッカーが再度開かれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## `$`インタラクティブシェルショートカットの改善

`$`インタラクティブシェルショートカットがエージェント処理中にも機能するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## スキルのモデル呼び出し無効化フラグの完全適用

スキルのdisable-model-invocationフラグが完全に適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## 言語サーバーシンボル不一致警告の実装

言語サーバーのシンボル不一致に対する警告が実装された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## ステアリング割り込みによるシェル出力待機の改善

ステアリング割り込みがシェル出力の待機を中断し、実行中のコマンドを終了させることなく処理できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## レスポンスリクエストサイズ制限の引き上げ

レスポンスリクエストのサイズ制限が引き上げられた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## プランモードのセッションフォルダ制限

プランモードでセッションフォルダ内のプランニングアーティファクトが許可される一方、セッションフォルダ外のファイル変更が制限されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## `/mcp add`および`/mcp edit`ウィザードの環境変数修正

`/mcp add`および`/mcp edit`ウィザードで環境変数値の`=`文字（base64パディングのシークレット/トークンに重要）が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## リモートセッションアップロードのリトライ修正

リモートセッションのアップロードがMission Controlの永続的な400/404レスポンスに対してリトライを停止するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## 設定フッターのタブ表示修正

`/settings`フッターのスコープ切り替え用タブ表示が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

## 大きすぎるツール結果画像のダウンスケール

大きすぎるツール結果画像がCAPI Responsesリクエストの互換性を維持するためにダウンスケールされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.74-1)

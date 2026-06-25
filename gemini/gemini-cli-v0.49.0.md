## GDC エアギャップサービスIDサポート

認証ライブラリ更新後のGDCエアギャップ環境でのService Identityサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27956)

## eval:inventoryコマンド

新しい`eval:inventory` CLIコマンドがレポートロジックとともに追加された。JSON出力にも対応。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28009)

## 静的eval解析器

静的evalソース解析器が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27631)

## ツール出力フォーマットの標準化

ツール出力のフォーマットが標準化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27772)

## ゼロクォータ制限のフェイルファスト

ゼロクォータ制限時にリトライループのハングを防ぐためにフェイルファストするようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27698)

## スキルインストール時のパストラバーサル防止

スキルインストール時のパストラバーサル脆弱性が防止された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27767)

## tmux偽陽性バックグラウンド検出の修正

tmuxでの偽陽性バックグラウンド検出が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27572)

## 設定マイグレーション

`coreTools`設定が`tools.core`にマイグレーションされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27947)

## ワークスペースパブリッシュとスケジューラの修正

ワークスペースのパブリッシュ失敗とスケジューラのイベントループスタベーションが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.49.0)

## NPMレジストリ認証の修正

NPMレジストリ認証の問題およびレジストリURLの末尾スラッシュ処理が修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.49.0)

## 依存関係の更新

Dependabotの14日間クールダウン期間が有効化され、npmパッケージの依存関係がピン留めされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.49.0)

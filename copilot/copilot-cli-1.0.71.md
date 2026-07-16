## Autopilotモードのバックグラウンドシェルハング修正

Autopilotモードがバックグラウンドシェルがターンより長く動作する場合にハングしなくなった。`COPILOT_TASK_WAIT_TIMEOUT_SECONDS` タイムアウトが適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /subagentsモデルピッカーの設定保持

`/subagents` のモデルピッカーを再度開いた際に、各エージェントのreasoning effortとコンテキストティアが保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## メモリコンテキストの30分更新

長時間実行セッションでメモリコンテキストが30分後に更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## MCPツールリストのサーバー変更時更新

MCPサーバーが変更された際にツールリストが最新の状態に保たれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 終了後のバックグラウンドgitプロセス残存修正

長時間実行されるバックグラウンドgitプロセスが終了後に残存しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## Ctrl+Rコマンド履歴の最大数設定

Ctrl+Rコマンド履歴の最大数が設定可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /voiceデバイスコマンドによるマイク選択

`/voice devices` コマンドが追加され、マイクの選択と永続化が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## Canvas対応の追加

拡張機能駆動のCLIインタラクションのためのCanvasサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## スラッシュコマンドの大文字小文字無視

スラッシュコマンドが大文字小文字に関係なくマッチするようになった（例：`/SESSION` が `/session` と同様に動作）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## ?キーの二度押しでヘルプ消去

`?` を2回押すとヘルプが消え、リテラルの `?` でプロンプトが開始されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## スクリーンリーダーのピッカー・モデル行フォーカス通知

フォーカスされたピッカーとモデル行に対するスクリーンリーダーのアナウンスが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## プランモードのワークスペース変更ツールブロック

プランモードが、ワークスペースを変更する組み込みツールをブロックするようになった。エージェントはファイルの編集や変更コマンドの実行ができなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 無効化スキルのcopilot skill list表示

無効化されたスキルが `copilot skill list` の出力でマーク表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 組み込みエージェントのタスク・サブエージェント利用制限

組み込みエージェントのタスクやサブエージェントへの利用可能性が制限された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## カスタムエージェントのシェルツールエイリアス対応

シェルツールをエイリアスでリクエストするカスタムエージェントが、対応するread、list、stopツールを受け取るようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## サブエージェントネスト深度のデフォルト引き下げ

サブエージェントのネスト深度デフォルトが6から4に引き下げられた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## サイドバーセッションの再起動間永続化

サイドバーセッションが再起動をまたいで永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## セッションの作業ディレクトリ紐付け

セッションがプロンプト、再起動、ワークスペースツール全体にわたって作業ディレクトリに紐付けられるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## Autopilot切替時の同一ターン質問自動回答

ターン中にAutopilotに切り替えた場合、同一ターンの質問が自動回答されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## バックグラウンドセッションの切替時維持

切り替え時にバックグラウンドセッションが存続し続けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 同期セッションの名前による再開

同期セッションを名前で再開する際に誤マッチが発生しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## GitHub MCPツールセット設定のsettings.json永続化

GitHub MCPのツールセット/ツール設定が `settings.json` 経由で永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## plugins marketplaceサブコマンドの追加

`plugins marketplace` サブコマンドが追加され、マーケットプレイスのリスト、追加、削除が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## リポジトリ有効プラグインの表示

リポジトリで有効なプラグインが `/plugin list` とスキルピッカーに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## マーケットプレイスプラグインインストール時のGit認証ヘルパー

マーケットプレイスプラグインのインストール時にGit認証ヘルパーが利用可能なまま維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## --add-github-mcp-tool '*'による全ツール有効化

`--add-github-mcp-tool '*'` を使用してすべてのGitHub MCPツールを有効化できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /chronicleコストチップの拡充

`/chronicle` のコストチップがローカルとクラウドのより豊富なコストプロファイルで拡充された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## Markdownでのインライン16進カラーハイライト

Markdown内のスタンドアロン16進カラーがインラインでハイライト表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /worktreeと/moveコマンドの追加

`/worktree` がコミットされていない変更を残して新しいworktreeを作成するようになった。新しい `/move` コマンドで変更を引き継ぐことが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## シェル補完の位置引数候補

シェル補完が位置引数の候補を提案するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## モデルピッカーのAutoモデル説明改善

モデルピッカーでAutoモデルの説明がMarkdownで表示され、クリック可能なLearn Moreリンクが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 不正なカスタムエージェントのエラー表示改善

不正なカスタムエージェントのロードエラーが明確に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## --share/--share-gist失敗時の非ゼロ終了

プロンプトモードで `--share` または `--share-gist` エクスポートが失敗した場合に非ゼロで終了するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## NO_COLOR環境変数の適用修正

`NO_COLOR` 環境変数がキャッシュされたchalkカラーレベルがある場合でも適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /settings変更後のセッションオプション即時適用

`/settings` の変更後にセッションオプションが即座に適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## モデルピッカーの検索結果なし時reasoning effort変更修正

モデルピッカーで検索結果がない場合に非表示モデルのreasoning effortが変更される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /cdのファイル・アクセス不能ディレクトリ切替防止

`/cd` がファイルやアクセス不能なディレクトリへの切り替えを防止するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## クイックヘルプオーバーレイ消去時の?残留修正

クイックヘルプオーバーレイを閉じた際にプロンプトに `?` が残る問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## プラグインコマンドエラーの重複Error:修正

プラグインコマンドの失敗で重複した「Error:」プレフィックスが表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## シェル補完のサブコマンドフラグ値提案修正

シェル補完がフラグ値としてサブコマンドを提案する問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 空のuntrackedファイルの追加行表示修正

空のuntrackedファイルが幽霊の追加行なしでレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## write(path)拒否の指定パス限定

`write(path)` の拒否が指定されたパスのみをブロックするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## Fish補完の列挙値制限

Fish補完が閉じた選択肢のフラグに対して列挙値のみを提供するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## --sandbox/--no-sandboxの対話的起動時警告表示

`--sandbox` と `--no-sandbox` が対話的起動時に無視される場合に警告が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## ピン留めプロンプト設定の追加

`/settings` にピン留めプロンプト設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /settingsダッシュボードのリポジトリスコープタブ追加

`/settings` ダッシュボードにRepoおよびRepo (local)スコープタブが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /usageアクティビティグラフの単数メッセージカウント表示

`/usage` アクティビティグラフが単数のメッセージカウントを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## カスタムエージェント名の隠しファイルパターン拒否

カスタムエージェント名で隠しファイルパターンが拒否されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## --allow-tool/--deny-toolの不正パターンエラー表示

不正な `--allow-tool` および `--deny-tool` パターンがエラーメッセージで拒否されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /tasksのシェル出力保持

完了したタスクの `/tasks` Shell Detailsにシェル出力が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## /mcp サーバー詳細の完全コマンド表示

`/mcp` サーバー詳細ビューで引数を含む完全なコマンドが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## 新規セッションのデフォルトディレクトリ開始

新規セッションがアクティブセッションのcwdではなくデフォルトディレクトリで開始されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

## copilot update/updateの"stable"チャネルオプション

`copilot update` および `/update` が「stable」をチャネルオプションとして受け入れるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.71)

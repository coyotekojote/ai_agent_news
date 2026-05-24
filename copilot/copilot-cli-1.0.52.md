## 非インタラクティブサブコマンドのstdin消費停止

`plugin list`、`mcp list`、`help`、`version`などの非インタラクティブサブコマンドがstdinを消費しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## 垂直スクロールバーの追加

メインの会話ビューにマウスドラッグ対応の垂直スクロールバーが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## Autopilotモードのパーミッションプロンプト修正

Autopilotモードに切り替えた際にツール、パス、URLのアクセスに対して予期しないパーミッションプロンプトが表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## セッション再開時のブランチ・gitコンテキスト更新

`copilot --continue`で保存されたディレクトリからセッションを再開する際にブランチとgitコンテキストが正しくリフレッシュされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## killコマンド安全フィルターの改善

シェルリダイレクト構文（`kill -0 <PID> 2>/dev/null`など）を含む有効なコマンドがkillコマンドの安全フィルターで誤って拒否される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## セッションの作業ディレクトリ復元

セッションが保存された作業ディレクトリで再開されるようになった。`-C <dir>`フラグでオーバーライドが可能。`--attachment`や`--log-dir`などの相対パス値を持つフラグも保存された作業ディレクトリから解決される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## コンテキストウィンドウティア選択の強制

コンテキストウィンドウティア選択（デフォルト約200K vs 1Mトークン）がエンドツーエンドで強制されるようになり、ティアの選択がコンパクション、トランケーション、トークン表示に正しく反映されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## AI Credits使用量の表示修正

Responses API使用後のセッションでAI Credits使用量が正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## tmux環境でのレンダリング改善

Cygwinまたはminttyでのtmuxでのレンダリングスタッターが解消された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## スラッシュコマンドピッカーのラベル表示改善

スラッシュコマンドピッカーで行が選択された際に(experimental)および(staff)ラベルのオレンジ色が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## 推論トークンの表示改善

推論トークンがトークン使用量サマリーで出力トークン数の括弧付き表示として表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## セッションファイルの破損エラー修正

URL/URIフィールドに非URL文字列を含むイベントがあるセッションが「Session file is corrupted」エラーなしで再開されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## HTTP/2アップロードのリトライ改善

HTTP/2アップロードの停滞によりタイムアウトしたリクエストが自動的にHTTP/1.1でリトライされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## Windowsでのセッション読み込み修正

Windows上でプロセスがハイビット終了コード（.NETの未処理例外など）で終了した場合にセッションの読み込みが失敗する問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## UIの改善

タイムラインエントリのコネクタカラーが展開時に周囲の要素と一致するようになった。truecolorをサポートしないターミナルでユーザーメッセージの背後にグレーの背景バーが表示されなくなった。ピッカーのチェックボックスが単一セルの▣/▢グリフに変更され、よりタイトで一貫した表示になった。`/statusline`ピッカーのアイテム説明がクリーンになり、スペーシングが改善された。終了サマリーの`AI Credits`ラベルが正しいスペーシングで表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## ステータスラインコマンドの拡張

ステータスラインコマンドが実行可能スクリプトパスに加えてプレーンシェルコマンドもサポートするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## プロセスログの自動プルーニング

起動時に`~/.copilot/logs/`から古いプロセスログファイルが自動的に削除され、ディスク使用量の無制限な増加が防止されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## カスタムエージェントの遅延ツール読み込み

カスタムエージェントがエージェントフロントマターの`deferred-tool-loading`によるオプトイン遅延ツール読み込みをサポートするようになり、大規模なツールリストを持つエージェントでのツール検索ディスカバリーが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## /restartと/updateのセッションID保持

`/restart`および`/update`が再起動後も現在のセッションIDを保持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## MCP OAuth設定キーのマイグレーション

MCPサーバー設定のレガシーなネストされた`oauth.clientId`および`oauth.callbackPort`キーがサポートされている`oauthClientId`および`auth.redirectPort`キーに自動マイグレーションされるようになった。MCP OAuthの再認証が設定された`redirectPort`を尊重するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## PowerShellの除算演算子の誤検知修正

Windows上でPowerShellの除算演算子が誤ってディレクトリアクセスプロンプトをトリガーする問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## /compactのフォーカス指示対応

`/compact`がオプションのフォーカス指示を受け付けるようになり、コンパクションサマリーの内容を指定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## 汎用サブエージェントのモデル更新

汎用サブエージェントが利用可能な場合にGPT-5.4またはGPT-5.5を使用するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## /usageのクォータプログレスバー

`/usage`がセッションおよび週間制限のクォータプログレスバーを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

## AI Creditsエラーメッセージの改善

AI Creditsのエラーメッセージがより明確な文言に更新され、「Manage budget」リンクが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52)

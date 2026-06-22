## 会話スクロールバー非表示設定の追加

会話のスクロールバーを非表示にする設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## CLI でのインライン画像レンダリング

CLI でインライン画像のレンダリングが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## スキルの argument-hint フロントマターサポート

スキルで argument-hint フロントマター機能がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## OpenTelemetry: コンパクション後チャットスパンの属性追加

成功したコンパクション後のチャットスパンに `gen_ai.conversation.compacted=true` 属性が付与されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## リモートエクスポートフラグのヘルプ出力改善

`--remote-export` および `--no-remote-export` フラグがヘルプ出力に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## コンパクトタイムラインの長いコマンド表示改善

展開されたコンパクトタイムラインで長いシェルコマンドや説明が折り返し表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## Markdown テーブルリンクのクリック対応

Markdown テーブル内のリンクがクリック可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## /usage のモデルごとトークン合計表示

`/usage` でモデルごとのトークン合計が表示されるようになり、大規模履歴のスキャンも高速化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## OpenTelemetry GenAI スパンの reasoning level 出力

OpenTelemetry の GenAI チャットスパンが `gen_ai.request.reasoning.level` を出力するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## オートパイロットモードのタスク完了後の動作変更

オートパイロットモードがエージェントのタスク完了後にインタラクティブモードに戻るようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## PowerShell コマンドレットの不要なディレクトリプロンプト修正

PowerShell コマンドレットが不要なディレクトリアクセスプロンプトを発生させる問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## 非インタラクティブプロンプト出力の整列修正

非インタラクティブプロンプトの出力が列1に整列されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## ビジョン無効時のキュー画像クリア

ビジョンが無効化された際にキューに入ったツール画像がクリアされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## モデル変更の適用完了待機

モデル変更が適用完了を待機するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## シェル安全プロンプトの 2>/dev/null リダイレクト処理修正

シェル安全プロンプトが `2>/dev/null` リダイレクトを読み取り専用として正しく扱うようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## 外部エディタプロンプトの改行正規化

外部エディタで編集されたテキストが LF に正規化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## フル許可セッションでの computer-use 同意スキップ

フル許可セッションで computer-use の同意プロンプトがスキップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## /clear 後のリモートエクスポート継続

`/clear` コマンド後もリモートエクスポートが継続し、セッション情報がタスク URL を維持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## セッション削除後のカーソル位置修正

セッション削除後のカーソル位置が正しく保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## musl ホストでの Linux libc ターゲット解決修正

musl ホストでの Linux libc ターゲットの解決が正しく行われるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## マルチセレクトプロンプトの空選択許可

minItems が未設定の場合、マルチセレクトプロンプトで空の選択が許可されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## アタッチ/リストア後のタイムライン表示修正

アタッチ/リストア後にホームセッションのタイムライン表示が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## /settings 検索の readline 編集サポート

`/settings` 検索で readline 編集とカーソル移動がサポートされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## OpenTelemetry のキャッシュ・reasoning トークンメトリクス修正

OpenTelemetry の GenAI スパンが正しいキャッシュおよび reasoning トークンメトリクスを出力するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## 終了時のターミナルモード無効化修正

終了時にターミナルモードが適切に無効化され、マウスホイールの問題が防止されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

## /rewind ファイルリストアダイアログのクリッピング修正

`/rewind` のファイルリストア確認ダイアログがフル高さで表示され、クリッピングが発生しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-2)

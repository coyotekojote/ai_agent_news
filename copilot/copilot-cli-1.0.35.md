## スラッシュコマンドのタブ補完

スラッシュコマンドが引数やサブコマンドのタブ補完に対応した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## セッションセレクターの改善

セッションセレクターにブランチ名とアイドル/使用中ステータスが表示されるようになり、検索機能も改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## `Ctrl+Y` による補完選択

補完オプションの選択に `Tab` の代替として `Ctrl+Y` が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## タブナビゲーションの Home/End キー対応

タブナビゲーションで `Home`/`End` キーがサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## 絵文字・マルチコードポイント文字の入力改善

テキスト入力における絵文字およびマルチコードポイント文字のハンドリングが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## セッション管理サブコマンド

`/session delete`、`delete`、`delete-all` サブコマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## 名前付きセッション

`--name` フラグでセッションに名前を付け、`--resume=<name>` で名前を指定してレジュームできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## 一時的な I/O エラーの表示改善

一時的な I/O エラーがタイムラインに赤いエラーエントリとして表示されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## セッショントークンの自動期限管理

セッショントークンの自動期限切れ処理が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## シェルエスケープコマンドの改善

シェルエスケープコマンド（`!`）が `/bin/sh` の代わりに `$SHELL` 環境変数を使用するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## `COPILOT_GH_HOST` 環境変数

GitHub ホスト名を指定する `COPILOT_GH_HOST` 環境変数がサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## Linux クリップボードユーティリティのエラーメッセージ改善

Linux でクリップボードユーティリティが見つからない場合のエラーメッセージが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## ユーザー設定の保存先変更

ユーザー設定が `~/.copilot/settings.json` に保存されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## パターン固有のインストラクションファイル

パターン固有のインストラクションファイルが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## HTTP フックの JSON ペイロード対応

HTTP フックが JSON ペイロードに対応した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## LSP サーバーのタイムアウト設定

LSP サーバーのタイムアウト設定オプションが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## 自己修正カスタムツール呼び出し

カスタムツール呼び出しの自己修正機能が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## grep/glob ツールの複数パス対応

grep および glob ツールが複数の検索パスを受け付けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## MCP サーバー名のスペース対応

スペースを含む MCP サーバー名がサポートされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## オートモードのレートリミット処理

オートモードでのレートリミットハンドリングが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

## バグ修正

- Windows でのツール可用性検出が修正された
- プラグインのインストールが再起動不要になった
- 大量テキスト表示のパフォーマンスが改善された
- 各種起動・シャットダウンの改善
- モデル変更通知で変更前後のモデル名が表示されるようになった
- `/update` と `/version` コマンドが設定された更新チャンネルに従うようになった
- `/usage` コマンドに GitHub スタイルのコントリビューショングラフが追加された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.35)

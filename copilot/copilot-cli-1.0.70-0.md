## プラグインのコミットSHA固定

プラグインソース設定の`sha`フィールドを使用して、プラグインを特定のコミットSHAに固定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## `--sandbox`/`--no-sandbox`フラグの追加

現在のセッション内でOS レベルのシェルサンドボックスを一時的に制御するための`--sandbox`および`--no-sandbox`フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## `/refine`コマンドの追加

雑なプロンプトを明確で構造化されたものに書き換える`/refine`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## `/settings`と`/model`への`--repo`/`--local`フラグ追加

`/settings`および`/model`コマンドに`--repo`と`--local`フラグが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## タイムラインタイムスタンプの表示設定

タイムラインのタイムスタンプの表示/非表示を制御する設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## リポジトリレベルの設定固定

`.github/copilot/settings.json`を通じて、モデル、エフォートレベル、コンテキストティア、URL/MCP/スキル拒否リストをリポジトリレベルで固定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## ライブセッション中のMCPサーバー管理API

ライブセッション中にアクティブなMCPサーバーを管理するためのSDK APIが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## GPT-5.6のツール駆動プログレスコメンタリー改善

GPT-5.6モデル向けのツール駆動プログレスコメンタリーのガイダンスが強化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## Markdownリンクのクリック対応

タイムラインとツール出力全体でMarkdownリンクとベアURLがクリック可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## エンタープライズ管理設定の定期リフレッシュ

エンタープライズの管理設定が長時間セッション中に毎時リフレッシュされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## MCPサーバーのサンドボックスステータス表示

ローカルに起動されたMCPサーバーが`/mcp list`でサンドボックスステータスを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## `/user`切り替え後のモデル表示修正

`/user`切り替え後にアクティブユーザーのモデルが正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## 拡張機能権限プロンプトの修正

拡張機能の権限プロンプトを拒否してもツール承認がブロックされなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## バックグラウンドエージェント通知の冗長排除

冗長なバックグラウンドエージェント通知が排除された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## 認証エラーメッセージの改善

起動時の認証エラーメッセージが`copilot login`への案内を正しく表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## プラグインキャッシュの再同期修正

プラグインキャッシュが欠落または空の場合の再同期が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## ユーザー認証のランタイム再起動間の永続化

ユーザー認証がランタイム再起動を跨いで永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## リモートターミナルでのブラウザ起動防止

リモートターミナルでブラウザが起動されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## ツールイベント順序と権限プロンプト修正

ツールイベントの順序と権限プロンプトのシーケンスが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

## Windowsデスクトップ通知のクラッシュ修正

Windowsデスクトップ通知のクラッシュが解消された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.70-0)

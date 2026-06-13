## ダイアログスクロールの改善

聞き返しやエリシテーションのダイアログがタイムラインと一緒にスクロールされるようになり、画面を占有しなくなった。エージェントの出力が常に視認可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## プラグイン拡張のマーケットプレイス対応

プラグインがエクステンションを同梱できるようになり、プラグインマーケットプレイスからインストール可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## /appスラッシュコマンドの追加

`/app`スラッシュコマンドが追加され、GitHubアプリまたはブラウザフォールバックを開けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## サブエージェントの設定機能

サブエージェントのモデル、推論エフォート、コンテキストティアをユーザー設定または`/subagents`（`/agents`）ピッカーから設定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## MCPサーバー設定のピッカーベースフロー

MCPサーバーの設定フォームがピッカーベースのフローに再設計され、使いやすくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## diffビューのコンテンツ検索

diffビューにコンテンツ検索機能が追加され、マッチハイライトとn/Nによるナビゲーションが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## 推論サマリーの空白行保持

推論サマリーセクション間の空白行が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## ライトテーマの背景色修正

ライトテーマのセカンダリ背景色のレンダリングが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## PowerShellリダイレクトパスの修正

PowerShellのリダイレクトパスがコンテンツ除外拒否を誤ってトリガーしなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## WebSocketトランスポートの修正

WebSocketトランスポートがTokioランタイム外でもクリーンにクローズするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## シェルツールエラーメッセージの改善

シェルツールのエラーメッセージが、シェルIDの停止・完了・回収の状態を明確に説明するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## 音声ランタイムダウンロードダイアログの修正

音声ランタイムのダウンロードダイアログがインストール失敗後に再表示ループに陥る問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## ストリーミングテキストの重複修正

ストリーミングされたアシスタントテキストが間欠的に重複表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## grepの欠落パス処理

grepが欠落パスをスキップして有効な結果で処理を継続するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## リモートMCP OAuthサーバーの起動修正

リモートMCP OAuthサーバーがマッチする設定ごとに一度だけ起動するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## プラグインフックの修正

プラグインフック（preToolUse、permissionRequest）が正しいペイロードで正しく発火するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.62)

## Claude Fable 5モデルのサポート

Claude Fable 5モデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## /settingsインタラクティブダイアログの追加

`/settings`インタラクティブダイアログが導入され、すべてのユーザー設定を一箇所で閲覧・編集できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## /agentsピッカーとエージェント作成ウィザードの改善

`/agents`ピッカーと「Create New Agent」ウィザードが統一されたボーダー、ヘッダー、一貫したスタイルの入力フィールドで洗練された。`/`キーでエージェント名によるフィルタリングが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## 自然言語スケジューリングの追加

`/every`および`/after`コマンドが`/experimental`スラッシュコマンドリストでアクセス可能になった。cron式、カレンダー時刻、または相対的な期間を使用した自然言語でのタスクスケジューリングがサポートされた。`beepOnSchedule`設定でスケジュール実行完了時のビープ音を無効化できる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## /worktreeコマンドの追加

`/worktree`コマンド（エイリアス`/move`）が追加され、git worktreeを作成して切り替えられるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## MCP・サーバー統合の強化

`.github/mcp.json`ワークスペース設定ファイルからMCPサーバーが自動ロードされるようになった。Geminiモデルがnullableスキーマ型のMCPツールで正しく動作するようになった。MCP OAuth再認証でリモートサーバーの保存済みOAuthクライアントIDが正しく使用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## mTLSおよびプライベートCA対応のOTLPテレメトリ

OTLPテレメトリのHTTPSエクスポートでmTLSとプライベートCAがサポートされた。標準OTelプロトコル環境変数によるhttp/protobuf OTLP HTTPエクスポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## 検索の高速化

大規模モノレポでのgrep検索がインデックス化された検索エンジンを使用して大幅に高速化された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## ターミナル・シェルの改善

WSLとtmuxセッションで色が正しくレンダリングされるようになった。空のプロンプトでEscまたはCtrl+Cを押してシェルモードを終了できるようになった。Bashツールでマルチバイトのステルス文字（emダッシュ、カーリークォートなど）が正しく処理されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## UIテーマの改善

ライトテーマのセカンダリ背景色が正しくレンダリングされるようになった。GitHubテーマがライトターミナルで本格的なGitHub Primerライトカラーパレットに適応するようになった。フルスクリーンスクロールバー機能が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## セッション管理の修正

セッション再開時に画面が空白になるバグが修正された。メモリ無効状態でのローカルセッション再開時にUIがクラッシュしなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## シェルコマンドバリデーションの修正

文字列リテラルや埋め込みドキュメントに「kill」のような単語が含まれる無害なコマンドがブロックされる誤検知が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## 安定性の向上

不正なUTF-8、過大な文字列バッファ、ターミナル切断エラーによるクラッシュが防止された。既存リンク内のGitHub issue/PR参照が壊れたネストされたオートリンクを生成しなくなった。パーミッションダイアログが閉じた後に貼り付けた画像がメインプロンプトに漏出しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

## その他の改善

`/sessions`がオーバーレイではなくSessionsタブに直接ナビゲートするようになった。`/fork`で「Creating fork...」進捗通知が表示されるようになった。`/env`出力で内部フックが非表示になりフックソースのフルパスが表示されるようになった。`/help`にユーザーレベルの指示ファイルの場所が表示されるようになった。ホームタブバーの表示、順序、非表示タブが`tabs`設定で構成可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.61)

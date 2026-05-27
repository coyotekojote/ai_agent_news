## フック進捗ストリーミング

長時間実行フックからリアルタイムのステータスメッセージをタイムライン内に表示するフック進捗ストリーミング機能が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## pluginDirectoriesサポート

`session.create`および`session.resume` RPCで`pluginDirectories`パラメータがサポートされ、SDKクライアントがOpen Plugins形式のディレクトリをセッションごとに読み込めるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## リモートセッション削除

セッションピッカーから直接リモートセッションを削除できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## マーケットプレイスプラグインのref指定

マーケットプレイスプラグインの追加時に`owner/repo#ref`構文がサポートされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## tmux 3.6bペイン進捗連携

プログレスインジケーターがtmux 3.6bのペイン進捗状態と連携するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## プラグインスキルの優先順位

プラグインディレクトリのスキルがパーソナルホームのスキルより優先されるようになった（プロジェクト > プラグインディレクトリ > パーソナル > カスタムの順）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## 推論トークン数の表示

セッションのトークンサマリーに推論トークン数が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

## バグ修正

スケジュールマネージャーのヒントバーテキストのフォーマットが修正された。`copilot update`および`copilot version`でリリースAPIリクエストが認証されるようになり、共有NAT環境でのレート制限が防止された。Diffビューのキーボードショートカットヒントが正しく表示されるようになった。Waylandコンポジターでクリップボードペーストが動作するようになった。インタラクティブシェルツールが親ターミナルのカラー設定を保持するようになった。オプショナルスキーマを持つCanvasツールがバリデーションエラーなしで開けるようになった。拡張機能のサブプロセスでコマンドフォーマットエラーが発生しなくなった。設定マイグレーションでレガシーのsnake_caseキーからのユーザーデータが保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.55-3)

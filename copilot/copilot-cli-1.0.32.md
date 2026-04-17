## セッション ID の短縮プレフィックス対応

`--resume` および `/resume` で完全なセッション ID の代わりに 7 文字以上の 16 進プレフィックスでセッションを指定できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## リモートセッションへの直接接続

新しい `--connect` フラグにより、セッション ID を指定してリモートセッションに直接接続できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## セッションアイドルタイムアウトの設定

`--session-idle-timeout` でセッションのアイドルタイムアウトが設定可能になった。デフォルトでは無効。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## 自動モデル選択

モデル選択で `auto` を指定すると、Copilot が最適なモデルを自動的に選択するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## 使用量制限の警告通知

週次使用量制限の 75% および 90% に達した際に警告通知が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## ドキュメントファイルの添付

プロンプトにサポート対象のドキュメントファイルを添付し、エージェントの分析・推論に利用できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## デバッグ情報フラグの追加

新しい `--print-debug-info` フラグにより、バージョン、ターミナル機能、環境変数を表示できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## GitHub Enterprise Cloud 認証の修正

`copilot login --host` が GitHub Enterprise Cloud (GHE) インスタンスで正しく認証されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## エージェントコンテキストへの日時情報追加

エージェントのコンテキストに現在の日時とローカルタイムゾーンオフセットが含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

## バグ修正

- `/clear` 後にステータスラインに不要な Unicode グリフが表示される問題を修正（Neovim 等のターミナル）
- `/cd` でディレクトリ変更後にリワインド機能が正しく動作するよう修正
- `/plan` およびプランモード使用時の複数行入力が保持されるよう修正
- 入力が空の場合のみ `Backspace` でシェルモードを終了するよう修正
- `/ask` ダイアログでマウスホイールスクロールが動作するよう修正
- テーブルの列幅、絵文字サポート、リサイズ時のボーダー安定性を修正
- レート制限時にセッションが一時停止しキュー内メッセージを自動リトライするよう修正
- トークン制限を超えるスキルが名前で検出・呼び出し可能な状態を維持するよう修正
- エージェント思考中のターミナルプログレスインジケーターの表示を修正
- 書き込み権限のないディレクトリでの `/feedback` バンドル保存を TEMP に変更

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.32)

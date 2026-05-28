## プラグイン・Git改善

`github`/`git`プラグインマーケットプレイスソースに`skipLfs`オプションが追加され、クローンおよびアップデート時にGit LFSのダウンロードをスキップできるようになった。npmグローバルインストールで自動更新ができない場合にワンタイム通知が表示されるようになり、`/doctor`で修正方法が確認可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 環境変数・シェル改善

ステータスラインコマンドに`COLUMNS`および`LINES`環境変数が渡されるようになり、ターミナル幅に応じたサイズ調整が可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsの改善

ディスパッチ入力のオートコンプリートがネイティブスラッシュコマンドやバンドルスキルも提案するようになった。PR列でPRが1つの場合は`PR #N`、複数の場合は`N PRs`と表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 診断・通知の改善

`claude doctor`が最後の更新試行結果を表示するようになった。MCPサーバーとコネクターの「認証が必要」通知が1つのメッセージに統合された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## macOSバックグラウンドセッション

バックグラウンドエージェントがmacOSの「プライバシーとセキュリティ」に「Claude Code」として表示され、アップグレード間で権限付与が維持されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

ステートフルMCPサーバーの再接続ループ（v2.1.147でのリグレッション）、カスタムAPIゲートウェイへの誤った認証情報送信、サブエージェントフロントマターMCPサーバーの設定無視、Windows PowerShellインストーラーの偽完了報告、`claude update`のリリースチャネル無視、セッション再開時の過大メモリ使用、バックグラウンドセッションの各種問題（`/bg`でのレスポンス消失、`/btw`キーボードショートカットの無応答、削除済みワーキングディレクトリのエラー表示など）が修正された。`/model`がセッション既定として保存されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

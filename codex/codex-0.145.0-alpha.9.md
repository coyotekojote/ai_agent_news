## アプリサーバー経由の環境ステータス公開

実験的な`environment/status`リクエストが追加され、環境を開始せずに設定済み環境を検査できるようになった。準備状態（ready、pending、disconnected、unknown）がエラー詳細とともに報告される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.9)

## ページネーションスレッド履歴のSQLiteマテリアライズ

ページネーションされたロールアウトレコードが、turns、items、projection progressの再構築可能なSQLiteテーブルに投影されるようになった。カーソルベースのローカル読み取りが実装された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.9)

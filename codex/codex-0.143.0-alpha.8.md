## ロールアウト永続化バイトの計測

1%サンプリングのロールアウト永続化メトリクスが追加され、ポリシー選択によるクラウドストレージへの影響を推定するためのアイテムごとのタグ付きJSON バイト合計が記録されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29498)

## 現在時刻リマインダーの経過時間ベースデバウンス

`reminder_interval_model_requests` が `reminder_interval_seconds` にリネームされ、リクエストごとではなく設定された経過時間後にリマインダーが挿入されるようになった。

[参考リンク](https://github.com/openai/codex/pull/29659)

## InvalidStreamErrorの詳細なUI伝播

`InvalidStreamError`の詳細情報がUIに伝播されるようになり、空のレスポンスに対してより具体的なエラーメッセージとガイダンスが表示されるようになった。`MAX_TOKENS_EXCEEDED`、`SAFETY_BLOCKED`、`RECITATION_BLOCKED`、`OTHER_BLOCKED`、`THINKING_ONLY_RESPONSE`、`NO_RESPONSE_TEXT`などのエラータイプが個別に処理される。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.1)

## ストリーム失敗時の履歴自動ロールバック

ストリームが失敗した際に自動的に履歴がロールバックされるようになり、不完全なターンがチャット状態を汚染することが防止された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.1)

## コンテキスト対応のリトライロジック

モデル回復のためのシステムインストラクション調整を含む、コンテキスト対応のリトライロジックが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.1)

## セマンティックバリデーションエラーのテレメトリ追跡

セマンティックバリデーションエラーの追跡がテレメトリに追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.1)

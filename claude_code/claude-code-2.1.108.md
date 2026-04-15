## プロンプトキャッシュ機能の拡張

API キー、Bedrock、Vertex、Foundry において、プロンプトキャッシュの TTL を 1 時間に延長できる環境変数 `ENABLE_PROMPT_CACHING_1H` が追加された。また、キャッシュを 5 分間に強制する `FORCE_PROMPT_CACHING_5M` も追加。`DISABLE_PROMPT_CACHING*` 環境変数によってキャッシュが無効化されている場合、起動時に警告が表示されるようになった。さらに、`DISABLE_TELEMETRY` を有効にしたサブスクリプションユーザーが 1 時間キャッシュではなく 5 分キャッシュにフォールバックしてしまう不具合を修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション Recap（要約）機能の追加

セッションに戻った際に文脈を提供する「recap」機能が追加された。`/config` から設定でき、`/recap` コマンドで任意のタイミングで呼び出すことも可能。テレメトリが無効な場合は `CLAUDE_CODE_ENABLE_AWAY_SUMMARY` を使って有効化できる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /resume ピッカーの改善

`/resume` が既定でカレントディレクトリのセッションを優先表示するようになり、`Ctrl+A` で全プロジェクトのセッションも参照可能に。`claude --resume <session-id>` で `/rename` による名前・色のカスタム設定が失われる問題、`--teleport` と `--resume <id>` のプリコンディションエラーで何も出力されず終了してしまう問題も修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## モデルとスラッシュコマンドの拡張

モデルが Skill ツール経由で `/init`、`/review`、`/security-review` といった組み込みスラッシュコマンドを自ら発見・呼び出せるようになった。`/undo` が `/rewind` のエイリアスとして利用可能に。`/model` コマンドは会話の途中でモデルを切り替える前に警告を出すよう改善。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エラーメッセージと UX の改善

サーバー側のレートリミットとプラン利用量リミットを区別して表示するようにエラーメッセージを改善。5xx/529 エラー時には `status.claude.com` へのリンクを表示。未知のスラッシュコマンドを入力した際には、最も近いコマンドを候補として提示するようになった。2.1.105 で発生した `/login` コード入力プロンプトに貼り付けができないリグレッションも修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## メモリ使用量の削減とバグ修正

言語グラマーを必要な時だけロードするように変更し、ファイル読み込み・編集・シンタックスハイライトのメモリフットプリントを削減。Agent ツールが auto モード時に安全性分類器のトランスクリプトがコンテキスト長を超えると権限確認を求めてしまう問題、`CLAUDE_ENV_FILE` が `#` コメントで終わる場合に Bash ツールの出力が空になる問題、`language` 設定時にダイアクリティカルマークがレスポンスから欠落する問題、ポリシーで管理されたプラグインが別プロジェクトから自動更新されない問題などを修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

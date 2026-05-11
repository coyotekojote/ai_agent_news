## Python SDKのターン通知IDルーティング

Python SDKでターン通知がIDごとにルーティングされるようになり、単一クライアントで複数のアクティブターンを同時にストリーミングできるようになった。`MessageRouter` がリクエストごとのレスポンスキューとターンごとの通知キューを管理する。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## TUIのテキスト折り返し改善

URLを含む行でワード境界が正しく保持されるようになり、トークンの途中で分割されなくなった。ブロッククォートやリスト、インデントされたコンテンツの左マージンが継続行でも維持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## ライトモードの選択コントラスト改善

TUIコントロールの選択ハイライトが背景に応じたアクセントスタイルを適用するようになった。ライト背景では暗めのシアン、ダーク背景では明るいシアンを使用し、視認性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## フックの信頼フロー改善

起動時に新規・変更されたフックのレビュープロンプトが表示されるようになった。保留中のフックをすべて一括で信頼するキーボードショートカットが追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## 大規模サブエージェント展開時のTUI応答性改善

同期的な `thread/read` 呼び出しがローカルレシーバースレッドキャッシュに置き換えられ、大規模なサブエージェントのファンアウト時にUIがフリーズしなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## ChatWidgetの状態管理リファクタリング

モノリシックなウィジェット状態管理が、入力キュー・ターンライフサイクル・トランスクリプト管理・ステータス・コネクタ・レビューモード・プロトコルディスパッチなどの専門モジュールに分割された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

## サービスティア設定の正規化

設定永続化時にサービスティアの値が正規化されるようになった。`priority`/`fast` は `"fast"` にマッピングされる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.131.0-alpha.5)

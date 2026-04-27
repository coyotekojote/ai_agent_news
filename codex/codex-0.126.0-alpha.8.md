## 巻き戻しプレビューの修正

新しい TUI セッションでユーザーメッセージが存在しない場合に Esc を 2 回押すと巻き戻しトランスクリプトオーバーレイが表示される問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/19510)

## シェルモードコマンドのプロンプト履歴永続化

シェルコマンド（`!` プレフィックス付き）がプロンプト履歴に先頭の `!` 付きで保持されるようになり、セッション間で呼び出しが可能になった。ラベルも「Bash mode」から「Shell mode」に更新された。

[参考リンク](https://github.com/openai/codex/pull/19618)

## 委任パッチ承認の詳細レンダリング

委任エージェントが進行中のファイル変更の承認をリクエストした際に、親 TUI が非アクティブスレッドからのリクエストを正しく処理・表示するようになった。

[参考リンク](https://github.com/openai/codex/pull/19709)

## プラグイン・アプリ・スキルハンドラーの整理

プラグイン、アプリ、スキルのハンドラーで繰り返されていた send_error/return ブランチが整理され、成功パスの可読性が向上した。

[参考リンク](https://github.com/openai/codex/pull/19490)

## 認証ロードの非同期化

codex-login、app-server 起動、CLI/TUI/exec インターフェースを含む認証ロード機構全体が非同期処理に変換された。

[参考リンク](https://github.com/openai/codex/pull/19762)

## 動的遅延ツールのフィルタリング修正

動的遅延ツールが `ToolRouter` 作成時に `model_visible_specs` からフィルタリングされるようになり、ToolRouter に依存するすべてのリクエストで問題が解消された。

[参考リンク](https://github.com/openai/codex/pull/19771)

## バグ修正・改善

- アカウントハンドラーとコマンドハンドラーがリファクタリングされ、リクエスト境界で一度だけ結果を計算・送信するようになった
- npm ステージングスモークテストのバージョンが 0.115.0 から 0.125.0 に更新された
- Bazel CI ジョブのセットアップがアーカイブされた setup-bazelisk から bazel-contrib/setup-bazel v0.19.0 に移行された

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.126.0-alpha.8)

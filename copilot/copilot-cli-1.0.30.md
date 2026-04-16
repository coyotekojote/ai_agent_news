## `/statusline` コマンドの追加

ステータスバーに表示する要素（ディレクトリ、ブランチ、エフォート、コンテキストウィンドウ、クォータ情報）をカスタマイズできる `/statusline` コマンド（`/footer` エイリアス付き）が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.30)

## `/undo` コマンドの改善

Git リポジトリ外やコミットが存在しない場合など、Rewind 機能が利用できない際に `/undo` コマンドが説明メッセージを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.30)

## プラグインディスカバリーの修正

`skills.discover` 機能利用時にプラグインのスキルとコマンドが正しく検出されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.30)

## バグ修正

- フィードバックフォームが正しい GitHub リポジトリにリンクするよう修正された
- ブラケットペースト処理のリグレッションにより失われていたクリップボードからの画像ペースト機能が復元された
- 全プラットフォームで `Ctrl+V` と `Meta+V` の両方が画像ペーストをトリガーするようになった
- プロンプトモードで `--list-env` フラグが削除された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.30)

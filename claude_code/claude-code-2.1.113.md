## ネイティブバイナリの起動方式への変更

CLI がバンドルされた JavaScript ではなく、プラットフォームごとのネイティブ Claude Code バイナリ（オプション依存）を起動するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネットワークドメインブロック設定の追加

`sandbox.network.deniedDomains` 設定が追加され、`allowedDomains` のワイルドカードで広く許可している場合でも特定ドメインをブロックできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンモードの選択操作改善

フルスクリーンモードで `Shift+↑/↓` による選択範囲の拡張時、表示領域の端を超えるとビューポートが自動スクロールされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 複数行入力のカーソル操作改善

`Ctrl+A` と `Ctrl+E` が複数行入力で現在の論理行の先頭・末尾に移動するようになった（readline 準拠の動作）。Windows では `Ctrl+Backspace` で前の単語を削除できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 長い URL のクリック可能な表示

レスポンスや Bash 出力中の長い URL が折り返されてもクリック可能な状態が維持されるようになった（OSC 8 ハイパーリンク対応）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /loop コマンドの改善

`Esc` キーで待機中のウェイクアップをキャンセルできるようになり、ウェイクアップ時の表示が「Claude resuming /loop wakeup」に変更された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Control の強化

`/extra-usage` が Remote Control（モバイル/Web）クライアントから利用可能になった。Remote Control クライアントが `@` ファイル補完候補を照会できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /ultrareview の改善

並列化されたチェックによる起動の高速化、起動ダイアログへの diffstat 表示、アニメーション付きの起動状態表示が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのストール検知

ストリーミング中にストールしたサブエージェントが、無期限にハングするのではなく 10 分後に明確なエラーで失敗するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bash ツールの表示改善

コメントのみの最初の行を持つ複数行コマンドが、トランスクリプトにコマンド全体を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## cd コマンドのパーミッション改善

`cd <現在のディレクトリ> && git …` の実行時にパーミッションプロンプトが表示されなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セキュリティ強化

- macOS: `/private/{etc,var,tmp,home}` パスが `Bash(rm:*)` ルール下で危険な削除対象として扱われるようになった
- Bash の拒否ルールが `env`/`sudo`/`watch`/`ionice`/`setsid` でラップされたコマンドにもマッチするようになった
- `Bash(find:*)` の許可ルールが `find -exec`/`-delete` を自動承認しなくなった

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

- MCP の同時呼び出しタイムアウト処理の修正
- `Cmd-Backspace`/`Ctrl+U` でカーソルから行頭までの削除が正しく動作するよう修正
- インラインコードスパン内のパイプ文字によるマークダウンテーブルの崩れを修正
- 未送信テキストの入力中にセッション要約が自動起動する問題を修正
- `/copy`「Full response」のマークダウンテーブルの列揃えを修正
- サブエージェント表示中に入力されたメッセージがトランスクリプトに表示されない問題を修正
- Bash の `dangerouslyDisableSandbox` がパーミッションプロンプトなしでコマンドを実行する問題を修正
- `/effort auto` の確認メッセージの修正
- 「copied N chars」トーストが絵文字／マルチコードユニット文字を過大カウントする問題を修正
- Windows で `/insights` が `EBUSY` でクラッシュする問題を修正
- ワンショットスケジュールタスクの終了確認ラベルの誤表示を修正
- フルスクリーンモードでのスラッシュ/@補完メニューの位置を修正
- `CLAUDE_CODE_EXTRA_BODY` の `output_config.effort` による 400 エラーを修正
- `NO_COLOR` 設定時にプロンプトカーソルが消える問題を修正
- 貼り付けされた MCP ツール名の `ToolSearch` ランキングを修正
- 長いコンテキストのセッション再開時の「Extra usage required」エラーを修正
- 依存関係バージョン競合時に `plugin install` が成功してしまう問題を修正
- 「Refine with Ultraplan」がリモートセッション URL を表示しない問題を修正
- SDK の画像コンテンツブロックが失敗しセッションがクラッシュする問題を修正
- Remote Control セッションがサブエージェントのトランスクリプトをストリーミングしない問題を修正
- Remote Control セッションの終了時のアーカイブ処理を修正
- Bedrock ARN 経由の Opus 4.7 で `thinking.type.enabled` の 400 エラーを修正

[参考リンク](https://code.claude.com/docs/en/changelog)

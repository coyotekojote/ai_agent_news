## `/resume` の大幅なパフォーマンス改善

大規模セッション（40MB 以上）での `/resume` が最大 67% 高速化された。デッドフォークエントリが多いセッションもより効率的に処理される。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## MCP 起動の高速化

複数の stdio サーバーが設定されている場合の MCP 起動が高速化された。`resources/templates/list` は最初の `@` メンション時まで遅延されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## フルスクリーンスクロールの改善

VS Code、Cursor、Windsurf ターミナルでのフルスクリーンスクロールがスムーズになった。`/terminal-setup` でエディタのスクロール感度を設定可能になった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## 思考インジケーターの改善

思考スピナーにインラインの進行状況メッセージ（「still thinking」「thinking more」「almost done thinking」）が表示されるようになり、従来のヒント行が置き換えられた。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `/config` 検索の拡張

`/config` 検索が設定名だけでなくオプション値にもマッチするようになった（例: 「vim」で検索するとエディタモード設定が見つかる）。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## `/doctor` コマンドの改善

Claude が応答中でもターンの完了を待たずに `/doctor` を開けるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## プラグイン依存関係の自動インストール

`/reload-plugins` およびバックグラウンドプラグイン自動更新で、既に追加済みのマーケットプレイスから不足しているプラグイン依存関係が自動インストールされるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## GitHub API レート制限の検出

Bash ツールで `gh` コマンドが GitHub の API レート制限に達した場合にヒントを表示し、エージェントがリトライではなくバックオフできるようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## 使用量タブの改善

Settings の使用量タブで 5 時間および週間の使用量が即座に表示されるようになり、使用量エンドポイントがレート制限されている場合にも失敗しなくなった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## エージェントフロントマターフックの修正

`--agent` でメインスレッドエージェントとして実行される際に、エージェントフロントマターの `hooks:` が発火するようになった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## セキュリティ修正

サンドボックスの自動許可が `/`、`$HOME`、その他の重要なシステムディレクトリを対象とする `rm`/`rmdir` の危険パス安全チェックをバイパスしなくなった。

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## バグ修正

- Devanagari およびその他のインド系スクリプトのターミナル UI での列アラインメントの崩れを修正
- Kitty キーボードプロトコルを使用するターミナル（iTerm2、Ghostty、kitty、WezTerm、Windows Terminal）で Ctrl+- によるアンドゥが機能しない問題を修正
- Kitty キーボードプロトコルを使用するターミナル（Warp フルスクリーン、kitty、Ghostty、WezTerm）で Cmd+Left/Right による行頭・行末ジャンプが機能しない問題を修正
- ラッパープロセス（`npx`、`bun run` 等）経由で起動した場合に Ctrl+Z でターミナルがハングする問題を修正
- インラインモードでターミナルリサイズや大量出力時にスクロールバックが重複する問題を修正
- 短いターミナル高さでモーダル検索ダイアログが画面からはみ出し、検索ボックスやキーボードヒントが隠れる問題を修正
- VS Code 統合ターミナルでスクロール中に空白セルやコンポーザ UI が消える問題を修正
- 並列リクエスト完了時のキャッシュコントロール TTL 順序に関する断続的な API 400 エラーを修正
- 50MB を超えるトランスクリプトの会話で `/branch` が拒否される問題を修正
- 大きなセッションファイルで `/resume` がロードエラーを報告せず空の会話を表示する問題を修正
- `/plugin` の Installed タブで「Needs attention」や「Favorites」に表示されているアイテムが重複表示される問題を修正
- セッション途中でワークツリーに入った後に `/update` および `/tui` が動作しない問題を修正

[参考リンク](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

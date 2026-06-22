## MCP サーバーの CLI 認証コマンド追加

`claude mcp login <name>` および `claude mcp logout <name>` コマンドが追加され、インタラクティブな `/mcp` メニューを開かずに CLI から MCP サーバーの認証が可能になった。また、SSH 経由での `--no-browser` stdin リダイレクトもサポートされた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフローエージェント詳細ビューのステータスフィルタリング

`/workflows` のエージェント詳細ビューで `f` キーを押してステータスフィルタリングが利用可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフローサブエージェントのスキーマバリデーション失敗時のループ修正

Workflow の `agent({schema})` サブエージェントがスキーマバリデーション失敗を繰り返した際に無限ループする問題が修正され、5回試行後に中止するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインの Skills セクション追加

`/plugin` の Installed タブに「Skills」セクションが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## iTerm2 teammate モード設定の追加

`teammateMode: "iterm2"` 設定が追加され、auto モードで `it2` CLI が見つからない場合に警告が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## AWS 認証情報の更新オプション

`/login` に「Claude Platform on AWS - refresh credentials」オプションが追加された（`awsAuthRefresh` 設定時）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## bash コマンド出力への自動応答

`!` bash コマンドの実行後、Claude が出力に自動的に応答するようになった。以前の動作（コンテキストのみ追加）を維持するには `"respondToBashCommands": false` を settings.json に設定する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スリープ復帰後のストリーミングエラー修正

マシンのスリープ復帰後にストリーミングリクエストが「Content block not found」や JSON パースエラーで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのトランスクリプトスクロール位置漏れ修正

サブエージェントのトランスクリプトのスクロール位置が終了時にメインのトランスクリプトに漏れる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドタスクプレビューの表示修正

バックグラウンドタスクのプレビューがエージェントのプランが読み込まれる前に未加工のツール名を一瞬表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Chrome タブグループの分離修正

同時 CLI セッションでプロダクト内パーミッションゲートがオフの場合に Chrome タブグループの分離が適用されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの要約重複修正

バックグラウンドセッションの要約が重複する問題が修正され、エージェント自身のターン終了時の要約が要約行として表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Agent deny ルールと allowed-types 制限の適用修正

`Agent(type)` の deny ルールおよび `Agent(x,y)` の allowed-types 制限が名前付きサブエージェントの生成時に適用されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドエージェント実行中の Esc/Ctrl+C 応答修正

メインターン終了後にバックグラウンドエージェントがまだ実行中の場合、Esc と Ctrl+C が応答しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## パーミッションプロンプトのオプション番号ずれ修正

パーミッションプロンプトでオプションテキストがオーバーフローした際にオプション番号がずれる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェントパネルの完了サブエージェント非表示修正

エージェントパネルで完了したサブエージェントの `x` ボタンを押しても非表示にならない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 古いセッション再開時の誤解を招く MCP 通知修正

古いセッション再開時に意図的に廃止されたツールに対して誤解を招く「MCP server disconnected」通知が表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /plugin Installed の「more above」インジケータ修正

`/plugin` Installed で既に最上部にスクロールしている場合に「more above」インジケータが表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 取り消し線の表示修正

アシスタントメッセージで `~~strikethrough~~` がリテラルなチルダとして表示され、取り消し線としてレンダリングされない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## --tools のフィーチャーゲートツール漏れ修正

コールドファーストランチ時にフラグ読み込み前に `--tools` がフィーチャーゲート付きツールを通過させる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agents のバックグラウンドジョブステータス修正

`claude agents` でバックグラウンドジョブに返信後も古い「needs input」メッセージが表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ライトターミナルでのダークテーマフラッシュ修正

ライトターミナルで `claude agents` からバックグラウンドセッションを開いた際にダークテーマが一瞬表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agents でのテキスト選択ハイライト修正

`claude agents` でマウス選択したテキストが削除後もハイライトされたままになる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッションコスト表示の修正

使用量ベースの Enterprise および Team サブスクライバーでセッションコストが表示されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## チームメイトの --effort レベル継承

エージェントチームにおいて、tmux/pane バックエンドで生成されたチームメイトがリーダーの `--effort` レベルを継承するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude mcp get/remove のタイプミス候補表示改善

`claude mcp get` および `claude mcp remove` でタイプミス時に最も近い設定済みサーバー名を提案するようになり、長いサーバーリストが省略されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MEMORY.md のコンパクト化リマインダー改善

エージェントがサイズ制限に近づいた際に `MEMORY.md` インデックスのコンパクト化を促すリマインダーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキルフロントマターのキー形式柔軟化

スキルフロントマターの `display-name`、`default-enabled`、`fallback`、`metadata.*` キーが kebab-case、snake_case、camelCase のいずれでも受け付けられるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 不正な SKILL.md YAML フロントマターのハンドリング改善

不正な `SKILL.md` YAML フロントマターがある場合、サイレントに失敗する代わりに空のメタデータでスキル本体が読み込まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## CLAUDE_CODE_MAX_RETRIES の上限変更

`CLAUDE_CODE_MAX_RETRIES` の上限が15に制限された。無人セッションでは代わりに `CLAUDE_CODE_RETRY_WATCHDOG` の使用が推奨される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドサブエージェントのパーミッションプロンプト改善

バックグラウンドサブエージェントが自動拒否する代わりにメインセッションにパーミッションプロンプトを表示するようになった。ダイアログにはどのエージェントが要求しているかが表示され、Esc でそのツールのみ拒否される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /review コマンドのエンジン統一

`/review <pr>` が `/code-review medium` と同じレビューエンジンを使用するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

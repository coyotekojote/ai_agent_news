## sandbox.credentials 設定の追加

`sandbox.credentials` 設定が追加され、サンドボックス化されたコマンドが認証情報ファイルやシークレット環境変数を読み取ることをブロックできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 組織設定によるモデル制限の追加

モデルピッカー、`--model`、`/model`、`ANTHROPIC_MODEL` に組織設定によるモデル制限が追加された。制限されたモデルを選択すると「restricted by your organization's settings」メッセージが表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フルスクリーンモードでのマウスクリック対応

フルスクリーンモードの選択メニュー（パーミッションプロンプト、`/model`、`/config` など）でマウスクリック選択がサポートされた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## --resume の "No conversation found" エラー修正

元の `-p` 実行でモデルターンが生成されなかった場合に `--resume` が「No conversation found」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 構造化出力の修正

`--json-schema` およびワークフロー `agent({schema})` の構造化出力が修正された。成功した `StructuredOutput` 呼び出し後にモデルが無制限に再呼び出しできなくなり、フォローアップターンでも確実に構造化出力が返されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモート MCP ツール呼び出しのタイムアウト修正

5分間応答がないリモート MCP ツール呼び出しが無期限にブロックする代わりにエラーで中止されるようになった。`CLAUDE_CODE_MCP_TOOL_IDLE_TIMEOUT` で上書き可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote セッション起動時間の改善

エージェントプロキシ CA のシステム信頼インストール追加後に Claude Code Remote セッションの起動が約2.7秒遅くなっていた問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 韓国語/CJK テキストの文字化け修正

ペーストをバイト単位の拡張キーイベントとして配信するターミナルで、韓国語/CJK テキストの貼り付けが文字化け（mojibake）になる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /update の Remote Control 経由でのハング修正

起動時信頼ダイアログが表示される場合に `/update` が Remote Control 経由でハングする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドジョブの "working" 無限表示修正

エージェントが構造化出力を生成せずにターンを終了した場合、agents ビューのバックグラウンドジョブが「working」のまま無限に表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## チャネル接続の切断修正

agents ビューへの移動後や `/bg`、`/tui`、`/update` 実行後にチャネル接続が切断される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント停止通知の改善

エージェント停止通知で誰がエージェントを停止したかが正しく表示されるようになり、表現が「finished」/「stopped」に改善された（以前は「came to rest」）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェント深度追跡の修正

再開されたサブエージェントが元のスポーン深度を復元し、フォークされたサブエージェントが深度上限にカウントされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント worktree 登録のリーク修正

強制終了されたエージェントからロックされた `.git/worktrees/` エントリが自動的にクリーンアップされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Ghostty での Cmd+click URL 開き修正

macOS の Ghostty でフルスクリーンモード時に Cmd+click で URL が開かない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude --help の --bg フラグ表示修正

`claude --help` に `--bg`/`--background` フラグが表示されていなかった問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /share アップロード中の Esc/Ctrl-C/Ctrl-D 修正

`/share` のアップロード中に Esc、Ctrl-C、Ctrl-D が動作しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /install-github-app の改善

GitHub Actions ワークフローのセットアップがオプションになり、GitHub App のみをインストールしてワークフロー/シークレットのステップをスキップできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /btw の矢印キーナビゲーション改善

`/btw` で ←/→ 矢印キーによる過去の回答のステップスルーが可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /plugin の未使用プラグイン表示改善

`/plugin` で最近使用していないプラグインが表示され、クリーンアップできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## [VSCode] 大規模セッション再開時の応答なし修正

大規模セッションの再開時に VSCode 拡張機能が応答しなくなる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

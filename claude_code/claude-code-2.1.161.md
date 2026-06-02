## OpenTelemetryメトリクスの改善

`OTEL_RESOURCE_ATTRIBUTES`の値がメトリクスデータポイントのラベルとして含まれるようになり、カスタムディメンション（チーム、リポジトリ）による使用量メトリクスのスライスが可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsの表示改善

`claude agents`の行が作業を分散している際に詳細の前に`done/total`を表示するようになった。peekでは最も実行時間の長いアイテムが表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPコネクタの表示改善

`/mcp`で未使用のclaude.aiコネクタが「Show unused connectors」行の下に折りたたまれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 並列ツール呼び出しの改善

並列ツール呼び出しで、失敗したBashコマンドがバッチ内の他の呼び出しをキャンセルしなくなった。各ツールが独立して結果を返すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## クリップボードの改善

フルスクリーンモードのクリップボードがLinuxで`wl-copy`/`xclip`/`xsel`を使用するようになった（利用可能な場合）。クリップボードとPRIMARYセレクション両方にコピーされ、ミドルクリックペーストが可能になった。「Hold `{key}` for native selection」のヒントがターミナルごとに正しいキーを表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アクセシビリティの修正

`/effort`ダイアログ、ワークフローアニメーション、プロンプトキーワードシマーが「Reduce motion」設定を尊重するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 管理設定ポリシーの修正

`forceLoginOrgUUID`/`forceLoginMethod`管理設定ポリシーがサードパーティプロバイダーセッション（Bedrock、Vertex、Foundry、Mantle）をorg pinと共にブロックしていた問題を修正（2.1.146でのリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## パイプ出力の修正

`--output-format text`または`json`で`claude -p`の標準出力がバックグラウンドサブエージェントの出力によって破損する問題を修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 各種バグ修正

- `/usage-credits`がTeam/Enterprise管理者に対して組織の使用設定ページではなく再ログインを開始する問題を修正
- `/autofix-pr`がgit worktreeや別リポジトリ内のセッションで「cannot run on default branch」と報告する問題を修正
- `--resume`ピッカーがgit worktree以外（例：jjワークスペース）のカレントディレクトリからのセッションを表示しない問題を修正
- WindowsフックでBashを明示的に呼び出す場合（例：`/usr/bin/bash script.sh`）に「command not found」や「cannot execute binary file」で失敗する問題を修正
- OpenTelemetryログイベント（`user_prompt`、`api_request`、`tool_result`、`tool_decision`）がテレメトリ初期化完了前に出力された場合にサイレントに破棄される問題を修正
- `claude mcp` list/get/addでシークレットが出力される問題を修正（`${VAR}`参照が展開されなくなり、クレデンシャルヘッダーとURLシークレットがマスクされるようになった）
- `isolation: "worktree"`で生成されたWorkflowエージェントがバックグラウンドセッションで自身のworktree内のファイル編集がブロックされる問題を修正
- `claude agents`からディスパッチされたバックグラウンドセッションがデーモン環境の古いモデルで起動し`settings.json`のモデルが無視される問題を修正
- セッション再開後にWriteツール結果のレンダリング時にクラッシュする可能性がある問題を修正
- エラー発生時に完了したサブエージェントが実行中として表示されたままになる問題を修正
- `CLAUDE_CODE_TMPDIR`が深いパスに設定されている場合に`$TMPDIR`配下のUnixソケットバインドで`EADDRINUSE`エラーが発生する問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)

## パフォーマンスの改善

レイアウトエンジンのJITコンパイルプロファイルの安定化により、ターミナルレンダリングパフォーマンスが向上した。大きなファイル書き込みのレンダリングパフォーマンスも改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## VSCode拡張の改善

ターミナルGPUアクセラレーションの無効化や`/terminal-setup`の実行を提案するヒントが追加され、文字化けの修正が案内されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

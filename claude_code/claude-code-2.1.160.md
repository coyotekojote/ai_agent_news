## セキュリティ強化

シェルスタートアップファイル（`.zshenv`、`.zlogin`、`.bash_login`）および`~/.config/git/`への書き込み前にプロンプトが表示されるようになった（意図しないコマンド実行の防止）。`acceptEdits`モードで、コード実行を許可するビルドツール設定ファイル（`.npmrc`、`.yarnrc*`、`bunfig.toml`、`.bazelrc`、`.pre-commit-config.yaml`、`.devcontainer/`など）への書き込み前にプロンプトが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Editツールの改善

`grep`でファイルを表示した後、別途Readを実行しなくてもEditが可能になった。単一ファイルの`grep`/`egrep`/`fgrep`がread-before-editチェックを満たすようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの修正

- `claude agents`から完了済みセッションを復元した際にチャット履歴が失われ元のプロンプトが再実行される問題を修正
- 夜間の退避後に再接続したバックグラウンドセッションで会話が失われ元のプロンプトが再実行される問題を修正
- `claude --bg`で負荷の高いマシンでバックグラウンドデーモンのコールドスタート時に「socket missing」エラーが発生する問題を修正
- 作業を再開したバックグラウンドエージェントがエージェントリストの「Completed」に表示される問題を修正
- バックグラウンドエージェントが非対応ターミナル（Apple Terminal、tmux）にターミナル同期出力マーカーを出力しレンダリングアーティファクトを引き起こす問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows関連の修正

- WSLでcopy-on-selectがWindowsクリップボードに書き込まれない問題を修正（OSC 52の代わりにPowerShell interopを使用）
- セッション開始ディレクトリが`claude rm`後もデーモン終了まで削除できない問題を修正
- 有効な`file:///C:/...`リンクがハイパーリンク対応Windowsターミナルで壊れたパスに書き換えられる問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)

## UIとレンダリングの修正

- `claude agents`でセッションリストに戻る際にオートアップデーターの再チェックにより数秒フリーズする問題を修正
- Escキー、矢印キー、タイピングがWindows上でバックグラウンドセッションやエージェントビュー接続時にCPU負荷が高い状態で無反応になる問題を修正
- エージェントリストからセッションを開いた直後にマウスホイールがトランスクリプトではなくプロンプト履歴をスクロールする問題を修正
- `claude agents`ビューでCJK IMEの変換候補が入力カーソルではなく左下に表示される問題を修正
- briefモードをオフにしてセッションを再開した際にClaudeの過去の返答がスクロールバックから消える問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードの修正

`v$`でヤンクしたレジスタを`p`で貼り付ける際、カーソル位置ではなく次の行に貼り付けられる問題を修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 音声モードの修正

プロジェクトディレクトリやブランチ名に非ASCII文字や特殊文字が含まれる場合に音声モードの接続が失敗する問題を修正。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エラーメッセージの改善

- サードパーティプロバイダー（Bedrock/Vertex/Foundry）でautoモード非対応メッセージが`CLAUDE_CODE_ENABLE_AUTO_MODE`を案内していた問題を修正
- `/effort ultracode`でモデルがxhighを実行できない場合にdynamic workflows設定を誤って指摘する問題を修正（サポート外モデルにはultracodeが提案されなくなった）
- SDK等CLI以外のホストで実行時にmodel-not-foundエラーが`--model`フラグを案内する問題を修正

[参考リンク](https://code.claude.com/docs/en/changelog)

## autoモードの改善

ルーチンアクションの推論を削減し、autoモード分類器のレイテンシが改善された。「could not evaluate this action」ブロックが減少した。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッション終了処理の改善

`claude rm`/`stop`およびアイドルリープ時に、SIGKILLの前にSIGTERMが実行中のシェルサブプロセスに送信されるようになり、クリーンアップハンドラが動作するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 設定変更

- `CLAUDE_CODE_OPUS_4_6_FAST_MODE_OVERRIDE`環境変数が削除された（no-opとなった）
- JetBrainsプラグインのインストール提案がスタートアップから削除された
- dynamic-workflowトリガーキーワードが`workflow`から`ultracode`に変更された（`workflow`ではトリガーされなくなったが、自分の言葉で依頼する方法は引き続き動作）。トリガーは紫色でハイライトされる。

[参考リンク](https://code.claude.com/docs/en/changelog)

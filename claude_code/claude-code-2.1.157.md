## プラグインの自動ロードとスキャフォールド

`.claude/skills`ディレクトリ内のプラグインがマーケットプレイスなしで自動的にロードされるようになった。`claude plugin init <name>`で`.claude/skills`に新しいプラグインの雛形を作成可能になった。`/plugin`引数のオートコンプリート（サブコマンド、インストール済みプラグイン名、既知のマーケットプレイスのプラグイン）が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsのエージェント設定対応

`claude agents`で`settings.json`の`agent`フィールドがディスパッチされたセッションに適用されるようになり、`--agent <name>`でオーバーライドも可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークツリーの改善

`EnterWorktree`がセッション中にClaude管理のワークツリー間を切り替え可能になった。Claudeが管理するワークツリーはエージェント完了時にアンロック状態のままとなり、`git worktree remove`/`prune`でクリーンアップ可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## テレメトリの拡張

`tool_decision`テレメトリイベントに`OTEL_LOG_TOOL_DETAILS=1`設定時に`tool_parameters`（bashコマンド、MCP/スキル名）が含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WSL画像貼り付け対応

WSLで画像貼り付け（`alt+v`キーバインド）、Windows 11でのスクリーンショット貼り付け、WindowsエクスプローラーからのD&Dによる画像取り込みに対応した。

[参考リンク](https://code.claude.com/docs/en/changelog)

## パフォーマンス改善

長い会話や再開した会話のパフォーマンスが、冗長なメッセージレンダリング再計算の排除により改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターミナル・UI改善

`/terminal-setup`がVS Code/Cursor/Windsurf統合ターミナルのGPUアクセラレーションを無効化してテキストレンダリングの乱れを防止するようになった。Feature of the Weekのクレジット取得ステータスがプロンプト上部の行ではなくステータスエリアの通知として表示されるようになった。「bash commands will be sandboxed」起動バナーが削除された（サンドボックス状態は`/status`やコマンドブロック時に引き続き表示）。「/ide for …」起動ヒントトーストが削除された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフロートリガー設定

プロンプト内の「workflow」という単語によるダイナミックワークフローのトリガーを制御する「Workflow keyword trigger」設定が`/config`に追加された。ワークフロートリガーキーワード直後のバックスペースでワークフローリクエストがキャンセルされるようになった（`alt+w`と同じ動作）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

処理不能な画像（ゼロバイト、破損）のペースト・MCP・ダイアログ経由での添付時にリクエストがクラッシュする問題、デスクトップアプリ・IDE拡張・SDK使用時のauto/bypass-permissionsモードでのサンドボックスネットワーク権限プロンプト表示、`claude agents`の完了セッション未退出、Escキーによるキャンセル不能、`.claude/worktrees/`配下のワークツリー孤立化、スリープ/ウェイク後の日付誤り、tmuxでのcopy-on-selectクリップボード不達、`--resume`のバックグラウンドサブエージェント未報告、セッションピッカーの残像、`--worktree`のルートディレクトリ誤り、`/model`ピッカーの不正なバージョンヒント、フルスクリーンモードでのMarkdownマーカー表示、managed-settings承認後のターミナルフリーズ、スクロールバックの重複行、VS Code等での右クリックペースト重複、IDEでのバックグラウンドサブエージェント停止不能、VS CodeでのOpus 4.8ファストモードインジケーター未表示などが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

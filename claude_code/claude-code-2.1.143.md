## プラグイン依存関係の強制

`claude plugin disable`が他の有効なプラグインが依存しているプラグインの無効化を拒否するようになった（コピー&ペースト可能な無効化チェーンのヒント付き）。`claude plugin enable`は推移的な依存関係を強制的に有効化する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインマーケットプレイスでのコンテキストコスト表示

`/plugin`マーケットプレイスのブラウズペインに、予測コンテキストコスト（ターンごと・呼び出しごとのトークン推定値）が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションのワークツリー分離無効化設定

`worktree.bgIsolation: "none"`設定が追加され、ワークツリーが実用的でないリポジトリでバックグラウンドセッションが`EnterWorktree`なしで直接ワーキングコピーを編集できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## PowerShellツールの改善

PowerShellツールが`-ExecutionPolicy Bypass`を渡すようになった。`CLAUDE_CODE_POWERSHELL_RESPECT_EXECUTION_POLICY=1`でオプトアウト可能。また、WindowsのBedrock、Vertex、Foundryユーザーに対してデフォルトで有効化された。`CLAUDE_CODE_USE_POWERSHELL_TOOL=0`でオプトアウト可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションのモデル・エフォートレベル保持

バックグラウンドセッションがアイドルからの復帰後に設定したモデルとエフォートレベルを保持するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## アタッチされたエージェントセッションでのShift+Tab改善

アタッチされたエージェントセッションでShift+Tabのサイクルにオートモードが含まれるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude agentsコマンドのフラグ拡張

`claude agents`が`--add-dir`、`--settings`、`--mcp-config`、`--plugin-dir`をダッシュボードとディスパッチされるバックグラウンドセッションに適用するようになった。さらに`--permission-mode`、`--model`、`--effort`、`--dangerously-skip-permissions`でディスパッチされるセッションのデフォルトを設定可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /bgコマンドの設定保持強化

`/bg`が`--mcp-config`、`--settings`、`--add-dir`、`--plugin-dir`、`--strict-mcp-config`を保持するようになり、バックグラウンドセッションがリスポーン後もMCPサーバーと設定を維持するようになった。また`--fallback-model`と`--allow-dangerously-skip-permissions`も保持されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの権限モード尊重

`claude agents`から起動されたバックグラウンドセッションが`settings.json`の`permissions.defaultMode`を尊重するようになった（以前はオートモードで上書きされていた）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークツリークリーンアップの安全性向上

ワークツリーのクリーンアップで`git worktree remove`が失敗した場合に`rm -rf`にフォールバックしなくなり、gitignoreされたファイルや作業中のファイルの損失が防止されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

破損した`.credentials.json`（`scopes`値が非配列）がCLI起動時のハングやOAuthトークンリフレッシュの無音中断を引き起こす問題が修正された。Windows TerminalとWSLでの`claude agents`の右クリックペーストが修正された。ストップフックが繰り返しブロックした場合に永久ループする問題が修正され、8回連続ブロック後にターンが警告で終了するようになった（`CLAUDE_CODE_STOP_HOOK_BLOCK_CAP`で上書き可能）。Claudeがイテレーション間でアイドル中にEsc/Ctrl+Cで`/loop`ウェイクアップをキャンセルできない問題が修正された。バックグラウンドシェルやサブエージェントの実行中に`/goal`エバリュエーターが発火する問題が修正された。`settings.json`の`env`で`NO_COLOR`/`FORCE_COLOR`がClaude Code自体のUI色を削除する問題が修正され、サブプロセスにのみ適用されるようになった。Windowsでセッション一覧表示時にエージェントビューがPowerShellプロセスを繰り返しスポーンする問題が修正された。プロンプトなしの`/bg`がフォークされたセッションに「continue」を送信する問題が修正され、入力待機するようになった。`--agent <name>`が`plugin:`プレフィックスなしでプラグイン提供エージェントを見つけられない問題が修正された。エージェントビューからのセッション削除がトランスクリプトファイルを削除しない問題が修正された。Windows Terminalでアタッチされたバックグラウンドセッションのスクロール時のステイルフラグメントレンダリングが修正された。ホストスリープやmacOS App Nap後のバックグラウンドエージェントの偽陽性ワーカー停滞検出ストームが修正された。5xxエラーメッセージがstatus.claude.comを指す代わりに設定されたゲートウェイやクラウドプロバイダを表示するようになった。macOSでフルディスクアクセスが付与されていてもバックグラウンドジョブセッションが`~/Documents`、`~/Desktop`、`~/Downloads`のファイル読み取りで「Operation not permitted」エラーが発生する問題が修正された。Windowsでレスポンスストリーミング中に`claude agents`で←を押すとエージェントリストが全入力に無反応になる問題が修正された。`~/.local/bin/claude`ランチャーが存在しないか実行不可能な場合にバックグラウンドデーモンのスポーンが実行中バイナリにフォールバックするようになった。`claude agents --allow-dangerously-skip-permissions`がディスパッチされたセッションを権限サイクルで利用可能にする代わりにバイパスモードにデフォルト設定する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

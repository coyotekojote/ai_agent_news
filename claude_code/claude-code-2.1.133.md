## ワークツリーのベース参照設定

`worktree.baseRef` 設定（`fresh` | `head`）が追加され、`--worktree`、`EnterWorktree`、およびエージェント分離ワークツリーが `origin/<default>` からブランチするか、ローカル `HEAD` からブランチするかを選択できるようになった。デフォルトの `fresh` により `EnterWorktree` のベースが `origin/<default>` に戻された（2.1.128 以降はローカル `HEAD` だった）。未プッシュのコミットを新しいワークツリーに保持するには `worktree.baseRef: "head"` を設定する必要がある。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## サンドボックスバイナリパスの設定

`sandbox.bwrapPath` および `sandbox.socatPath` マネージド設定が追加され（Linux/WSL）、カスタムの bubblewrap および socat バイナリの場所を指定できるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## 親設定の動作制御

`parentSettingsBehavior` アドミン層キー（`'first-wins' | 'merge'`）が追加され、管理者が SDK の `managedSettings`（親層）をポリシーマージにオプトインできるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## フックへの effort レベル提供

フックがアクティブな effort レベルを `effort.level` JSON 入力フィールドおよび `$CLAUDE_EFFORT` 環境変数経由で受け取れるようになった。Bash ツールのコマンドでも `$CLAUDE_EFFORT` を読み取れる。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## フォーカスモードの改善

フォーカスモードの動作が改善された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## メモリ使用量の改善

メモリプレッシャー時にウォームスペアのバックグラウンドワーカーを解放することで、メモリ使用量が改善された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## ヘルプ表示の改善

`claude --help` で `--remote-control` が `--remote-control-session-name-prefix` と並んで表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## 並行セッションの認証修正

リフレッシュトークンのレースにより共有クレデンシャルが上書きされ、並行セッションがすべて 401 でデッドエンドになる問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## Edit/Write 許可ルールの修正

ドライブルート（`C:\`）や POSIX `/` にスコープされた `Edit`/`Write` 許可ルールが正しくマッチせず、常にプロンプトが表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## ファイルロックのエラー修正

クロックスキューや低速ディスクによりヒストリーまたはセッションログファイルのロックが侵害された際の未ハンドル rejection（`ECOMPROMISED`）が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## 会話コンパクション中の Esc 修正

会話コンパクション中に Esc を押すと誤った「Error compacting conversation」通知が表示される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## MCP OAuth フローのプロキシ対応修正

`HTTP(S)_PROXY` / `NO_PROXY` / mTLS が MCP OAuth フロー全体（ディスカバリ、動的クライアント登録、トークン交換、トークンリフレッシュ）で尊重されない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## マップされたネットワークドライブの修正

`--add-dir` / SDK `additionalDirectories` 経由で渡されたマップされたネットワークドライブ上で Read/Write/Edit が拒否される問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## リモートコントロールの停止/中断修正

claude.ai からの Remote Control の停止/中断がローカルの Esc と同様に CLI セッションを完全にキャンセルしない問題が修正された。スタックしたツールやプロンプトを中断した後、キューに入ったメッセージが進まなくなっていた。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## effort レベルのセッション間干渉修正

`/effort` が一つのセッションで変更された際に他の並行セッションの effort レベルが予期せず変更される問題が修正された。IDE での effort 変更がサイレントにドロップされる関連問題も修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## サブエージェントのスキル発見修正

サブエージェントが Skill ツール経由でプロジェクト、ユーザー、またはプラグインのスキルを発見できない問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

## VSCode 拡張の修正

`claudeCode.claudeProcessWrapper` が拡張ビルドに Claude バイナリがバンドルされていない場合に「Unsupported platform」で失敗する問題が修正された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.133)

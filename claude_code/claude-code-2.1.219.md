## Claude Opus 5のデフォルトモデル化

Claude Opus 5（`claude-opus-5`）が追加され、デフォルトのOpusモデルとなった。1Mコンテキストウィンドウを持ち、ファストモードは$10/$50 per Mtokで利用可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サンドボックスネットワーク厳格許可リスト設定の追加

`sandbox.network.strictAllowlist`設定が追加された。サンドボックス化されたコマンドに対して、許可リストにないホストへのアクセスをプロンプトなしで拒否する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## DirectoryAddedフックの追加

`/add-dir`またはSDKの`register_repo_root`コントロールリクエストでセッション中に新しい作業ディレクトリが登録された後に発火する`DirectoryAdded`フックが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ヘッドレスストリームJSONのMCPサーバーエラー情報追加

ヘッドレスの`stream-json`初期化イベントに`mcp_server_errors`が追加された。`--mcp-config`エントリのうち設定バリデーションでスキップされたものがリストされ、ターミナル実行時には起動警告が表示される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフローサイズガイドライン設定の追加

`workflowSizeGuideline`設定キーが追加された。任意の設定ファイルからダイナミックワークフローサイズのガイドラインを設定可能。設定中は`/config`行が非表示になる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ネストされたサブエージェントのstream-json転送

深度2以上で生成されたサブエージェントが、`--forward-subagent-text`設定時にstream-jsonで表示されるようになった。生成元のAgent `tool_use` idをキーとして使用する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのネスト深度拡張

サブエージェントがデフォルトで深度3までネストされたサブエージェントを生成できるようになった（以前は1）。`CLAUDE_CODE_MAX_SUBAGENT_SPAWN_DEPTH=1`で無効化可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude -p`テキスト出力の修正

ストリーム途中のAPIエラーでターンが終了した際に、既に生成された回答がドロップされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/model`ピッカーの表示修正

統合されたOpus行が「Opus (1M context)」ではなく「Opus」と表示されるよう修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 権限承認の永続化修正

セルフホストランナーの再起動中に承認された権限がセッション再開時にドロップされる問題が修正された。承認されたアクションが確実に実行されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fableモデル表示の修正

含まれているプランでも古いキャッシュにより「Requires usage credits」と表示される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セルフホストランナーのSIGTERM処理修正

リース期限切れまでアクティブ行が残り続ける問題が修正され、クリーンに登録解除されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## GNU screenでのcopy-on-select修正

選択内容をコピーする代わりにbase64がターミナルに出力される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Remote Controlファストモードステータス修正

モデル切り替え、再接続、または組織チェック失敗後に古いステータスが保持される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WindowsのGitBashパス修正

`CLAUDE_CODE_GIT_BASH_PATH`がbash/shバイナリでない場合に終了またはbashとして使用される問題が修正され、警告付きで無視されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモード矢印キー動作修正

空のプロンプトで←を押した際、INSERTモードだけでなくNORMALモードからもエージェントビューに戻るよう修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スクリーンリーダーモードの入力修正

キーストロークごとに入力行全体が書き換えられる問題が修正され、入力した文字のみがエコーされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Opus 4.7のファストモード除外

`/fast`がOpus 5およびOpus 4.8に適用されるようになり、Opus 4.7は除外された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude-apiスキルの更新

Claude Opus 5がデフォルトとなり、Opus 4.8からの移行パスが提供された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エラーメッセージの改善

「Remote Control is only available via api.anthropic.com」エラーが、原因となった具体的な設定名を表示するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `claude --teleport`の改善

現在のチェックアウトが指すリポジトリがセッションのリポジトリと一致しない場合に、どのリポジトリを指しているかが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ダイナミックワークフローのデフォルトサイズ変更

ダイナミックワークフローがデフォルトで中サイズガイドライン（15エージェント未満を目標）になった。`/config`のDynamic workflow sizeで別のサイズまたは無制限を選択可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCP許可/拒否リストの解決方法変更

`${VAR}`エントリが設定ファイル環境ではなく、起動時の環境とマネージド設定の環境から解決されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/model`ピッカーのハイライト変更

最新モデルの名前のみがハイライトされるようになり、任意のサブセットではなく新しいリリースを示すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフローサイズインジケーターの追加

現在のデフォルトワークフローサイズが実行中のワークフローステータス行に追加され、`/config`へのポインターが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

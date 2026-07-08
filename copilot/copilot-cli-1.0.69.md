## サンドボックスポリシーバッジの変更

ビルトインのファイル編集にサンドボックス制限を回避するラベルとして「(sandboxed)」ではなく「(sandbox policy)」バッジが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/plugins`ダッシュボードの追加

プラグインのインストール管理のための`/plugins`ダッシュボードが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/mcp list`コマンドの追加

接続されたMCPサーバーとそのステータスを表示する`/mcp list`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## エージェント作業中の`/mcp`マネージャーアクセス

エージェントが作業中でも`/mcp`マネージャーにアクセスできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## プラグインMCPサーバーの重複警告

複数のプラグインが同じMCPサーバーを定義している場合に警告が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## LLM判定による自動承認モード

LLMが判断する自動承認モードが追加され、許容可能と判断されたリクエストが自動的に承認されるようになった。`stayInAutopilot`設定でオートパイロットの永続性を制御できる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## gemini-3.5-flashの最小推論エフォートサポート

gemini-3.5-flashに対する最小推論エフォートサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## サンドボックスバイパスの承認機能

`sandbox.allowBypass`が有効な場合、ユーザーがビルトインファイル編集のサンドボックスバイパスを一度だけ許可できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Web Fetchのサンドボックスネットワークポリシー準拠

Web Fetch操作がアクティブなサンドボックスネットワークポリシーに従うようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## セッション再開・切り替えの高速化

セッションの再開と切り替え操作が大幅に高速化された。二次的な処理の削除により高速化が実現された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/diff`レンダリング・スクロールの高速化

大きなdiffでの`/diff`のレンダリングとスクロールのパフォーマンスが大幅に改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## モデルピッカーの表示改善

タイムラインが混雑している場合もモデルピッカーが画面上に完全に表示されるようになり、詳細バナーの展開時に自動スナップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/model`ピッカーのスクロールバー追加

`/model`ピッカーリストにスクロールバーが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 推論エフォートラベルのフッター表示

CLIフッターに推論エフォートラベルが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/sandbox add-path`提案の改善

`/sandbox add-path`の提案がリクエスト時のみ開かれるように改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/chronicle cost-tips`のエビデンスベース推奨

`/chronicle cost-tips`がエビデンスに基づく推奨を含むように改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Alt/Optionスクロールによる1行移動

Alt/Optionキーを押しながらスクロールすることで1行ずつ移動できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## スラッシュコマンドピッカーの改善

タブ展開するターミナルでスラッシュコマンドピッカーの行が崩れないように改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## プラグインリロードのセッション再起動不要化

インストール済みプラグイン拡張機能がセッションの再起動なしでリロードできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## OAuth再接続時のMCPサーバーツール登録

OAuthゲート付きMCPサーバーが再接続後にツールを登録するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## スキル読み込みエラーの表示

スキルの読み込みエラーと警告がスキルリストに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 委任PRのデフォルトブランチ変更

委任PRがデフォルトで現在のブランチに対して作成されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## worktreeブランチからのPR検索

ローカルブランチ名が異なる場合でもworktreeブランチからPRを検索できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 自動承認タイムラインエントリのリクエスト件名表示

自動承認のタイムラインエントリにリクエストの件名が含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/allow-all auto`の実験モード必須化

`/allow-all auto`が実験モードを必要とするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 不活性なサンドボックスホストリストの削除

不活性なサンドボックスホストリストとClearポリシーの終了時トグルが削除された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 空プロンプトからのクイックヘルプ修正

空のプロンプトから余分な`?`なしでクイックヘルプを開けるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 空の`--name=`値の拒否

セッション開始時に空の`--name=`値が明示的に拒否されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## ダブルEscでのメインターン中断

ダブルEsc押下でメインターンの実行が中断されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Windowsの終了時クラッシュ防止

Windows終了時の無害なクラッシュレポートが防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Ctrl+Cでのask_userプロンプト解除

Ctrl+Cでask_userおよびelicitationプロンプトが解除されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/help`のrewind/undo重複表示修正

`/help`がrewind/undoを2回リスト表示する問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Waylandでの`/copy`フォールバック

Wayland環境で`/copy`が`wl-copy`にフォールバックするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## マークダウンのコロン保持修正

レンダリングされたマークダウン出力でコロンが正しく保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## macOSペーストボードのstderr抑制

クリップボード操作中のmacOSペーストボードのstderrが抑制されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## tmuxパススルーでのクリップボード書き込み

クリップボード書き込みがtmuxパススルーでラップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## WSL UNCパスの許可

ローカルファイルに対するWSL UNCパスが許可されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `--reasoning-effort`の確実な適用

CLI起動時に`--reasoning-effort`が確実に適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## サンドボックスuserPolicy設定の説明表示

サンドボックスuserPolicy設定に説明が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 無効化LSPサーバーの表示

`/lsp test`で無効化されたサーバーが無効として表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## Chronicleのローカルアシスタント使用量表示

ChronicleおよびセッションSQLで正確なローカルアシスタント使用量が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## モノレポでのtgrepインデクサーのメモリ不足防止

モノレポでtgrepインデクサーがメモリ不足になる問題が防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## リモートセッション作成の遅延

読み取り専用リモートセッションの作成が最初のメッセージまで遅延されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 異なるリポジトリからのリモートセッション再開確認

異なるリポジトリからリモートセッションを再開する前に確認が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## モデル切り替えの句読点対応修正

ツールコールIDに句読点が含まれる場合のモデル切り替えが正しく動作するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## MCP OAuth認証キャンセル後のステータス保持

OAuthキャンセル後にMCPサーバーがneeds-authステータスを保持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## スタッフ専用コマンドの事前認証ヘルプ非表示

スタッフ専用コマンドが事前認証ヘルプから非表示になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## CLIモデルピッカーの改善

CLIモデルピッカーでモデルのブラウズとフィルタリングがより簡単になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 静的コンテキストのプロンプトバジェット警告

静的コンテキストがプロンプトバジェットの大部分を使用している場合に警告が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## `/sandbox`パスエントリのファイル・フォルダ補完

`/sandbox`パスエントリにファイルとフォルダの補完が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## セッション分割ビューでのブランチラベル更新

バックグラウンドセッションのブランチラベルがセッション分割ビューで更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## 不要なMCPリロードのスキップ

読み込み済みセッションに戻る際の不要なMCPリロードがスキップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## バイパスモード無効時のオートパイロット権限プロンプトスキップ

バイパスモードが無効な場合にオートパイロット権限プロンプトがスキップされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

## デバッグログの完全収集

大きなファイルを切り詰めずにデバッグログが収集されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.69)

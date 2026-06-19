## `/branch` コマンドの追加

Claude Codeの命名規則に合わせて `/fork` のエイリアスとして `/branch` コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## 実験的ワークツリーフラグの追加

`--worktree [name]`（`-w`）フラグが追加され、`<repo>.worktrees/` 配下にgitワークツリーを作成・再利用できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## `/agent` 名のタブ補完

`/agent` コマンドでエージェント名のタブ補完が利用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## モデルファミリエイリアスの追加

opus、sonnet、haiku、gpt、geminiなどのモデルファミリエイリアスが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## Windows Terminal用Ctrl+Backspaceバインド

`/terminal-setup` にWindows Terminal向けのCtrl+Backspaceバインドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## リモートMCPサーバーのOAuthトークンサポート

ホスト提供のOAuthトークンをリモートMCPサーバーで利用できるSDKサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## 実験的コンパクトタイムライン機能

ツール呼び出しや推論の行を個別に展開・折りたたみできる実験的コンパクトタイムライン機能が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## セッションリジュームでの画像・PDF永続化

ソースファイルが変更されても、画像やPDF添付ファイルがセッションリジュームをまたいで永続化されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## タスク・探索サブエージェントの無効化オプション

ビルトインのタスクおよび探索サブエージェントを無効化できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## セッションリジューム時のレスポンス改善

大規模な履歴読み込み中もセッションリジュームのレスポンスが維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## コード検索とワークツリー一覧の高速化

コード検索およびワークツリー一覧表示のパフォーマンスが向上した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## シェルコマンドの構文ハイライト

タイムラインでシェルコマンドに構文ハイライトが適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## Canvas再接続時の保持

Canvasインスタンスが再接続やリスタートをまたいで保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## ステータスラインピッカーの色分け

ステータスラインピッカーのチェックボックスが有効時は緑、無効時はグレーで表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## システムライト/ダークモードの自動追従

システムのライト/ダークモード変更が自動的に追従されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## インラインコードのテーマ付きチップスタイル

Markdownのインラインコードがテーマ付きチップスタイルでレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## MCP組織ポリシー適用の修正

MCPサーバーの作成・リロード時の組織ポリシー適用が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## コンテンツ除外によるシェルコマンドブロックの修正

コンテンツ除外がシェルコマンドをブロックしなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## Alpine musl Linuxパッケージの修正

Alpine musl Linux向けパッケージのダウンロードが修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## オートパイロットモードの改善

オートパイロットモードがelicitation、ask_user、sampling、permission各プロンプトを自動処理するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## ターミナル報告カラースキームサポートの削除

ターミナル報告によるカラースキームサポートが廃止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.64-1)

## タイムラインでのツール呼び出し時間表示

タイムラインヘッダーに各ツール呼び出しの所要時間が右寄せで表示されるようになった。実行中（5秒以上）はライブでカウントされる。`/settings showToolDurations`で無効化可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## ファーストパーティプラグインの自動更新

セッション開始時にファーストパーティプラグインが最新バージョンに自動更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## 実験的な`/new-worktree`コマンド

新しいワークツリーを作成し、そのワークツリーで新しい会話を開始できる実験的な`/new-worktree`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## ログインフローの改善

TTYを持たないローカルデスクトップサブプロセス（IDE統合を含む）でブラウザフローがデフォルトとなった。リモートおよびヘッドレス環境では引き続きデバイスコードフローが使用される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## インタラクティブシェルショートカットの改善

「$」がアーム状態の際にEnterキーで起動し、インラインヒントが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## 拡張スラッシュコマンドの実行修正

複数の拡張がロードされている場合、拡張スラッシュコマンドが呼び出しごとに正確に1回だけ実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## インライン画像の表示修正

タイムラインがスクロールした際にインライン画像の最初の行が繰り返し表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## パイプstdinのフック動作

stdinでパイプされたプロンプトが`-p`フラグと同様に`sessionEnd`フックを扱い、完了したエージェントターンごとに発火するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## 分割ビューサイドバーのUX改善

閉じる確認が「x again to close」と表示され、ダブルプレスの要件が明確になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## トークン使用量の表示

ACPプロンプト結果とライブ通知にトークン使用量情報が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## マネージド設定の強制リフレッシュ

起動時にサーバー管理設定の新規取得を必須とする`forceRemoteSettingsRefresh`設定が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## サンドボックスバイパスのセッション制限

サンドボックスの無効化が現在のセッションにのみ適用され、新しいセッションではサンドボックスが再開されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## マネージド設定のフォールバック

サーバー取得に失敗した場合、永続キャッシュにフォールバックし、閉じた失敗ではなく開いた失敗になるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## サンドボックスバイパスの自動化

CLIがブロックされたコマンドをサンドボックス外で再実行することをモデルに相談せず自動的に提案するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## `/rewind`コマンドの強化

gitが不要になり、Copilotが変更したファイルのみを復元し、内容が一致しないファイルをスキップし、会話のみまたは完全復元の選択が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## `/permissions`コマンドの追加

承認モード間の切り替えが可能な新しい`/permissions`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## セッション切り替えの最適化

セッション切り替え時にMCPサーバーの再起動やフック状態の再構築が不要になり、セッション中断が防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## サンドボックスのツールチェーンキャッシュアクセス

サンドボックス内のビルドにツールチェーンキャッシュ/レジストリ/インストールへのアクセスを許可する`allowDevToolCaches`設定（デフォルト有効）が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## プログレッシブトランスクリプトレンダリング

長いセッションのトランスクリプトがプログレッシブにレンダリングされ、スクロールの応答性が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## 大規模トランスクリプトのパフォーマンス向上

セッション再開が大幅に高速化・軽量化された。230MB・74kイベントのトランスクリプトが約10秒から1秒未満で読み込まれ、ピークメモリが約25%削減された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

## 自動安全性ジャッジモデル選択

安全性ジャッジモデルが自動で選択されるようになり、`/allow-all`ジャッジがユーザー設定から除外された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.78)

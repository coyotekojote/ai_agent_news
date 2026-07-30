## プラグイン管理のenable/disableコントロール追加

`/plugins`でプラグイン、指示、エージェント、LSPサーバー、フックの有効化・無効化コントロールが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## grok-4.5モデルのサポート追加

grok-4.5モデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## セッションサイドバーの追加

複数の同時セッションを管理するためのSessionsサイドバーが追加された。セッション間の切り替え、新規セッションの作成、ステータスの確認が可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## ディレクタブルキューマネージャーの追加

キューに入れたメッセージの並べ替え、編集、削除、繰り返し、即時送信が可能なディレクタブルキューマネージャーが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## `/limits predict`コマンドの追加

類似セッションに基づいてAIクレジット制限を提案する`/limits predict`コマンドが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## カスタムステータスラインコマンドのタイマーリフレッシュ

カスタムステータスラインコマンドに設定可能なタイマーリフレッシュ機能が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## Rioターミナルでのインライン画像レンダリング

KittyグラフィックスをサポートするRioターミナルでインライン画像がレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## ボイスモードのメディア一時停止・再開

ボイスモードが録音前に再生中のメディアを一時停止し、録音後に再開するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## サンドボックス拒否パスの強制適用

macOS/Linuxで相対パスおよびシンボリックリンクのエントリに対してサンドボックス拒否パスが強制適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## エンタープライズ管理者によるサンドボックス制限の強制

エンタープライズ管理者がマネージド設定により制限的なサンドボックスフロアを強制できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## 未送信プロンプトテキストのセッション保持

未送信のプロンプトテキストが元のセッションに保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## セッション再開時のAutopilot/Planモード復元

セッション再開時にAutopilotおよびPlanモードの設定が復元されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## URL権限プロンプトの改善

URL権限プロンプトがサンドボックス警告とモデルの推論を保持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## `/diff`の大規模マルチファイル差分表示の高速化

`/diff`で大規模なマルチファイル差分がシンタックスハイライト付きでより高速に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## `web_fetch`のHTTPリダイレクト追従

`web_fetch`がHTTPリダイレクトを追従するようになり、リダイレクト時にエラーが発生しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## サイドバーのホバーフォーカス無効化

サイドバーのホバーによるフォーカスがデフォルトで無効化され、アクティブセッションカードがアクセント表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## サブエージェント完了後のセッション失敗の修正

サブエージェント完了後に「Holder terminated during creation」エラーでセッションが失敗する問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## 起動時のヒント表示の改善

Copilot指示がないリポジトリでのみ`/init`が提案されるように起動時のヒント表示が改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## フック出力の上限設定

メモリ消費を防ぐため、フック出力が1回の呼び出しにつき10MiBに制限された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## MCPツールの高速読み込み

定義スコープのスナップショットを使用してMCPツールがより高速に読み込まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## マウス設定の即時反映

マウス設定の変更がセッション中に即座に反映されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

## `/worktree`切り替え後の作業ディレクトリ修正

`/worktree`で切り替え後にセッションの作業ディレクトリが元のチェックアウトに戻ってしまう問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76)

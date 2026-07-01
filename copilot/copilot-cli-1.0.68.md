## kimi-k2.7-codeモデルのサポート

kimi-k2.7-codeモデルのサポートが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## IDE接続の一時切断時のツール可用性維持

一時的なIDE切断時にもツールが利用可能な状態を維持し、自動復旧するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## タブ補完でのスラッシュコマンドエイリアス表示

タブ補完でスラッシュコマンドのエイリアスがインラインで表示されるようになった（例：`/pr automerge|agentmerge`）。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## セッションディレクトリ削除時のフック修正

セッションディレクトリやgitワークツリーが削除された場合にフックがエラーを起こす問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## タイ語・デーヴァナーガリー文字の描画改善

クリップされた出力でのタイ語およびデーヴァナーガリー文字のレンダリングが改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## サンドボックス内のgitコマンド改善

サンドボックス環境内のリポジトリサブディレクトリからgitコマンドが実行可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## インタラクティブセッションのカーソル改善

インタラクティブセッションでデフォルトで縦棒カーソル（非点滅）が使用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## ネストされたサブエージェントのツールフィルター継承

ネストされたサブエージェントでツールフィルターが正しく継承されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## プランバジェットのステータスライン表示

対応プランにおいて、プランバジェットの詳細がステータスラインおよび`/usage`に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## エージェント画面からのセッション管理

エージェント画面からセッションの閲覧、再開、切り替えが可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## コードレビューのgit一時エラーリトライ

コードレビュー時のgitの一時的な失敗に対してリトライが実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

## その他の修正・改善

- MCP設定フォームでフォーカスフィールドに「❯」シェブロンインジケーターが追加された
- フッターのモデル表示が推論エフォートやコンテキストティアの変更時に同期されるようになった
- シンボリックリンクされたスキャンルートからの重複スキル・コマンドパースエラーが排除された
- `/cd`および`/worktree`コマンド後にセッションサイドバーのブランチが更新されるようになった
- Windows拡張長パスでのエージェント・インストラクション検出が有効化された
- macOSでタイムラインテキストコピー時のターミナル破損が防止された
- ファイル編集がサンドボックスのファイルシステムポリシー内に収まるよう保証された
- PowerShell変数参照に関するコンテンツポリシーの問題が解決された
- `/diagnose`セッションログ抜粋でのマルチバイト文字保持が修正された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.68)

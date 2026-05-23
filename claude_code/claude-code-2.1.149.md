## 使用状況の表示改善

`/usage`コマンドでスキル、サブエージェント、プラグイン、MCPサーバーごとのコスト内訳が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /diffビューのキーボードスクロール対応

`/diff`の詳細ビューで矢印キー、`j`/`k`、`PgUp`/`PgDn`、`Space`、`Home`/`End`によるキーボードスクロールがサポートされた。

[参考リンク](https://code.claude.com/docs/en/changelog)

## GFMタスクリストチェックボックスのレンダリング

Markdown出力でGFMタスクリストチェックボックス（`- [ ] todo` / `- [x] done`）がレンダリングされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エンタープライズ向けMCP設定

`allowAllClaudeAiMcps`マネージド設定が追加され、claude.aiクラウドMCPコネクターの読み込みが可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セキュリティ修正

PowerShellの組み込み`cd`関数によるパーミッションバイパスが修正された。gitワークツリーサンドボックスの書き込み許可リストが共有`.git`ディレクトリだけでなくメインリポジトリ全体をカバーしていた問題が修正された。PowerShellのプレフィックス/ワイルドカード許可ルールがネイティブ実行ファイルを事前承認しない問題が修正された。`PWD`/`OLDPWD`/`DIRSTACK`変数追跡のパーミッション分析ギャップが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正

Bashツールの`find`コマンドが大きなディレクトリツリーでmacOSのシステムファイル/vnodeテーブルを枯渇させる問題が修正された。マネージド設定の承認ダイアログが起動時に受け入れ後にターミナルがフリーズする問題が修正された。`/ultraplan`およびリモートセッション作成が「Could not capture uncommitted changes」で失敗する問題が修正された。シンキングスピナー、折りたたまれた出力の行数、スラッシュコマンド引数ヒント、ステータスバーの表示など、各種UI問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## デスクトップアプリ連携

TUIから`/app`コマンドでデスクトップアプリへのハンドオフが可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## リモートコンパクション時のツール出力リライト

リモートコンパクション中にサイズ超過のツール出力がリライトされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## Multi-Agent v2設定のカタログ化

Multi-Agent v2の設定がカタログとして管理できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## ローカル画像パスのモデル公開

ローカル画像パスがモデルに対して公開されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## EDUアカウントのクラウド設定バンドル対応

EDUアカウントがクラウド設定バンドルを取得できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## プロファイルスイッチャー

app-serverのアカウントセッションプロトコルが追加され、プロファイル切り替え機能の基盤が整備された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## git enrichmentのガード

git enrichment処理にガードが追加され、安全性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## バグ修正

推論エフォートのフォールバックショートカットが修正された。

`/goal`編集時のマルチラインペーストが修正された。

フォークされたスレッドの名前継承が修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

## インフラストラクチャの改善

macOSリリースアーティファクトのAzure Key Vaultによる署名が導入された。Windowsセットアップマーカーが完了シグナルとして使用されるようになった。Python SDKランタイムが0.137.0a4にピン留めされた。Pythonランタイムのリリースワークフローが分離された。ユーザーBazel設定がCodexワークツリーにコピーされるようになった。SandboxPolicyのexecスレッディングが簡素化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.138.0-alpha.1)

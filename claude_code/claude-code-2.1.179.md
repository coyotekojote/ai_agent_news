## ストリーム中断時の部分レスポンス保持

ストリーム中の接続切断時に部分レスポンスが保持されるようになり、生のエラー表示ではなく内容が保存されるようになった。「running tool」でスピナーがスタックする問題も修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WSL2でのマウスホイールスクロール修正

Windows TerminalおよびVS Code内のWSL2環境でマウスホイールスクロールが動作しない問題が修正された（2.1.172でのリグレッション）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Linuxサンドボックスのglob処理修正

大きなディレクトリツリーでの `denyRead`/`allowRead` glob処理によりBashツールの説明文が巨大になりセッションが使用不能になる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フィードバック調査の誤キャプチャ修正

ターン完了直後に1桁の返信がセッション評価として即座にキャプチャされるフィードバック調査の問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ウェルカム画面のバナー表示修正

ウェルカム画面で複数のプロモーションバナーが重なって表示される問題が修正され、セッションごとに最大1つのプロモのみ表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サブエージェントのCtrl+O修正

サブエージェント表示中にCtrl+Oを押してもサブエージェントのトランスクリプトが表示されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプト入力のフォーカス修正

プロンプト入力をクリックしてもサブエージェント/フッターパネルからフォーカスが戻らない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートセッションのバックグラウンドタスク表示修正

リモートセッションのバックグラウンドタスクがターン間で「still running」として表示され続ける問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## リモートセッションのプラグイン読み込み改善

リモートセッションでのプラグイン読み込みパフォーマンスが向上した。

[参考リンク](https://code.claude.com/docs/en/changelog)

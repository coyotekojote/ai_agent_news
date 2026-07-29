## ディレクタブルキューマネージャーの追加

新しい「staff」機能により、キューに入ったメッセージの並べ替え、編集、削除、再送、即時送信が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## セッションサイドバーの追加

複数の同時セッションを管理するための実験的なセッションサイドバーが追加された。セッション間の切り替え、新規セッションの生成、ステータスの監視が可能。`/experimental on`で有効化できる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## エンタープライズサンドボックスポリシーの強制

管理者がマネージド設定で制限的なサンドボックスポリシーを設定できるようになった。ユーザーのサンドボックス設定を緩和することなく強化する。`/sandbox`ダイアログでは組織設定のマネージド値がロックされたフィールドとして表示される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## サンドボックス検索のバイパスプロンプト改善

サンドボックス化された検索で即座にバイパスプロンプトが提供されるようになり、重複するバイパスプロンプトが防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## フック出力の上限設定

フック出力が1回の実行あたり10MiBに制限されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## Rioターミナルのインライン画像サポート

RioターミナルでKittyグラフィックスプロトコルによるインライン画像レンダリングがサポートされた。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## サブエージェント完了時のエラー修正

サブエージェント完了後に「Holder terminated during creation」エラーが発生する問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

## `/init`提案の改善

起動時のヒントで、既存のCopilot指示がないリポジトリでのみ`/init`が提案されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-2)

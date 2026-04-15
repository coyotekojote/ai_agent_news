## Escape キーによるプロンプト解除の安定化

Escape キーでプロンプトを確実に解除できるようになり、操作が固まってしまう問題が解消された。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## find -exec 実行時のディレクトリアクセス確認の抑制

`find -exec` の引数に対してディレクトリアクセス確認プロンプトが不要に発生していた不具合を修正。スクリプト実行時のノイズが大幅に減った。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## エージェントセッションのチェックポイント越えツール呼び出し対応

エージェントセッションにおいて、チェックポイントをまたぐツール呼び出しが正しく処理されるようになり、セッションエラーが解消された。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## Anthropic BYOM での画像データ取り扱い修正

Anthropic BYOM 経由でファイルを閲覧する際に、画像データが正しく含まれるよう修正された。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## Remote タブの Copilot コーディングエージェント対応

Remote タブが Copilot コーディングエージェントのタスクとステアリングに対応した。GitHub Web や GitHub Mobile アプリからも、実行中の CLI セッションを監視・操作できる。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## 指示ファイルの統合によるトークン削減

複数の指示ファイルを統合することで、不要なトークン消費を削減するように改善された。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

## ACP サーバーを localhost のみにバインド

セキュリティ強化のため、ACP サーバーが localhost のみをバインドするようになった。

[参考リンク](https://github.com/github/copilot-cli/blob/main/changelog.md)

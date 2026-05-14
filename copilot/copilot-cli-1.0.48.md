## モデルピッカーのトークン価格表示

トークンベース課金ユーザー向けに、モデルピッカーがドットインジケーターの代わりに実際のトークン価格を表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.48)

## 命令ファイルのglobパターン修正

applyToフロントマターで引用符なしのglobパターン（例: `applyTo: **/*.ts`）を使用した命令ファイルが正しく適用されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.48)

## CJK文字・絵文字の描画修正

CJK文字や絵文字を含む入力テキストが行間に空白のギャップなく描画されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.48)

## /contextのトークン制限表示修正

`/context`コマンドが常に128kと表示するのではなく、すべてのモデルに対して正しいトークン制限を表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.48)

## バグ修正

Azure DevOps専用ワークスペースにおいて、プロンプト/ヘッドレスモードで組み込みのgithub-mcp-serverが自動無効化されるようになった。ターミナルカーソルが装飾要素ではなく入力フィールドに正しく配置されるようになった。ACPクライアントがアクティブモデル変更時に更新された設定オプションを受け取るようになった。`/ask`ダイアログが受信できないフォローアップ返信のプロンプトを表示しなくなった。モデルに送信されるスキルコンテンツからYAMLフロントマターのメタデータが除外されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.48)

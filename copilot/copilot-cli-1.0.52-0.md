## カスタムエージェントの遅延ツール読み込みサポート

カスタムエージェントがエージェントフロントマターの`deferred-tool-loading`によるオプトイン方式の遅延ツール読み込みをサポートするようになった。広範なツールリストを持つエージェントに対してツール検索ディスカバリーが利用可能になる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## /compactコマンドのフォーカス指示対応

`/compact`コマンドがオプションのフォーカス指示を受け付けるようになり、コンパクション要約を精緻化できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## 汎用サブエージェントのモデルアップグレード

汎用サブエージェントがアクセス可能な場合にGPT-5.4またはGPT-5.5を利用するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## /usageコマンドのクォータ進捗バー表示

`/usage`コマンドがセッションおよび週間制限のクォータ進捗バーを表示するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## AIクレジットエラーメッセージの改善

AIクレジットのエラーメッセージがより明確な表現になり、予算管理リンクが含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## バグ修正

終了サマリーで「AI Credits」ラベルが適切なスペーシングで表示されるようになった。`/restart`および`/update`コマンドが再起動後に現在のセッションIDを維持するようになった。レガシーなネストされた`oauth.clientId`および`oauth.callbackPort`キーがサポートされる`oauthClientId`および`auth.redirectPort`キーにマイグレーションされるようになり、無視されなくなった。MCP OAuthの再認証が設定された`redirectPort`を尊重するようになった。WindowsでPowerShellの除算演算子が誤った「ディレクトリアクセスを許可」プロンプトを引き起こす問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.52-0)

## Amazon Bedrockのカスタムトランスポートサポート

ビルトインの`amazon-bedrock`プロバイダーで`base_url`、`auth`、`http_headers`をAWSプロファイルおよびリージョン設定と併用してオーバーライドできるようになった。カスタムエンドポイントでのコマンドベースのBearerトークン認証が可能になり、AWS署名をバイパスしつつ、標準Bedrockセットアップのリージョナルエンドポイント解決は維持される。以前の`credentialSource`列挙型が`usesCodexManagedCredentials`ブール値に置き換えられた。

[参考リンク](https://github.com/openai/codex/pull/33695)

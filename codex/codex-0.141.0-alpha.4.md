## プラグイン推奨システムの導入

エンドポイントベースのプラグイン推奨機能が追加された。推奨プラグインのエンドポイントキャッシュ、提案UIの汎用化、インストールスキーマの簡素化が含まれる。

[参考リンク](https://github.com/openai/codex/pull/27704)

## リモート環境cwdのネイティブレンダリング

リモート環境のカレントワーキングディレクトリがネイティブにレンダリングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/28152)

## ターミナルサブエージェントエラーの親エージェントへの伝播

ターミナルサブエージェントのエラーが親エージェントに表示されるようになり、デバッグが容易になった。

[参考リンク](https://github.com/openai/codex/pull/28375)

## マルチエージェントv2メッセージの型付きエンベロープ

マルチエージェントv2メッセージに型付きエンベロープのレンダリングが追加された。

[参考リンク](https://github.com/openai/codex/pull/28368)

## Bedrockクレデンシャルソースの公開

`account/read`でBedrockのクレデンシャルソースが公開されるようになった。

[参考リンク](https://github.com/openai/codex/pull/27751)

## サスペンド後のTUI復元

サスペンド（Ctrl+Z）後にTUIが正しく復元されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28342)

## exec-serverのファイルチャンクストリーミング

exec-serverがファイルをチャンク単位でストリーミングするようになり、大きなファイルの転送効率が向上した。

[参考リンク](https://github.com/openai/codex/pull/28354)

## ユーザーシェルコマンドのローカル環境使用

ユーザーのシェルコマンドがローカル環境で実行されるようになった。

[参考リンク](https://github.com/openai/codex/pull/28163)

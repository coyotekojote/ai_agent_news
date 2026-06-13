## プラグイン提案のリモートカタログ制限

アプリベースのプラグイン提案がリモートカタログに制限されるようになった。ローカルプラグイン提案はフォールバックおよび明示的に設定されたプラグインに限定された。

[参考リンク](https://github.com/openai/codex/pull/27988)

## プラグインマネージャーの認証モード対応

PluginsManagerに初期AuthModeパラメータが追加され、ChatGPT/SIWCベースのセッションとAPIキーログインセッションの区別が可能になった。

[参考リンク](https://github.com/openai/codex/pull/27652)

## プラグインMCPサーバーの認証ルートによるゲーティング

認証ルートに基づくプラグインMCPサーバーのゲーティングが実装された。SIWC/Codexバックエンド認証ではMCPサーバーが除外され、APIキー認証ではAppsが除外されるようになった。

[参考リンク](https://github.com/openai/codex/pull/27459)

## マネージドリモートコントロール無効化の強制

トップレベルの「allow_remote_control」要件パースが追加され、リモートコントロールを強制的にオフにするトランスポートポリシーが実装された。無効時にはすべてのremoteControl RPCコールがJSON-RPCエラーで拒否される。

[参考リンク](https://github.com/openai/codex/pull/27961)

## WebSocketでのリクエストスコープターン状態送信

WebSocketレスポンスリクエストでclient_metadataを介してターン状態が交換されるようになった。WebSocketの動作が既存のHTTPパス契約と同期された。

[参考リンク](https://github.com/openai/codex/pull/27996)

## コンパクトリクエストでのターン状態送信

ターンスコープのOnceLockがインラインv1コンパクションに直接渡されるようになった。プレターンコンパクトが後続のサンプリングのための状態を確立できるようになった。

[参考リンク](https://github.com/openai/codex/pull/28002)

## Hermetic Wineテストサポートの追加

Bazelで管理されるx86_64 Wineプリビルトによるクロスプラットフォームテストが導入された。exec-serverのクロスOS統合テストが可能になった。

[参考リンク](https://github.com/openai/codex/pull/27964)

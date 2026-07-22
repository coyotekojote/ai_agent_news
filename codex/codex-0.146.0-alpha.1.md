## Gitプラグインのコミットハッシュ検証

Gitプラグインソースで解決されたHEADコミットが要求されたSHAと一致しない場合に拒否されるようになった。ブランチ名の衝突が防止される。

[参考リンク](https://github.com/openai/codex/pull/34644)

## レスポンスアイテムIDの常時割り当て

すべてのセッション（ストリーム、フォーク、コンパクト、非OpenAI）でクライアント作成のレスポンスアイテムにIDが割り当てられるようになった。`features.item_ids`は設定可能な機能として廃止された。

[参考リンク](https://github.com/openai/codex/pull/34645)

## 認証ルーティングへのプロキシポリシー伝播

アプリケーションの解決済みプロキシポリシーが、不在設定フォールバックに依存するのではなく、認証/ログイン/クラウドフローに明示的に伝達されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34649)

## AuthManagerのルーティング設定必須化

AuthManager/AuthConfigの構築時に`AuthRouteConfig`が必須となった。解決済みルーティング設定がすべてのプロダクション呼び出し元を通じて渡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34650)

## コアテストサポートの共有HTTPクライアント移行

core_test_supportの直接reqwest依存がcodex-http-clientに置き換えられた。

[参考リンク](https://github.com/openai/codex/pull/34651)

## 外部環境パスのターン差分レンダリング修正

外部環境からのパスを使用した際のターン差分のレンダリングが修正された。

[参考リンク](https://github.com/openai/codex/pull/34654)

## 認証リフレッシュのプロキシルート設定適用

認証リフレッシュリクエストが設定されたプロキシルーティングを適切に尊重するようになった。

[参考リンク](https://github.com/openai/codex/pull/34655)

## スレッドフォーク時の承認レビュアー保持

スレッドがフォークされた際に承認レビュアーのコンテキストが維持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34664)

## LM Studioリクエストの共有HTTPクライアント経由化

LM Studioプロバイダーのリクエストが共有HTTPクライアントインフラストラクチャを使用するよう移行された。

[参考リンク](https://github.com/openai/codex/pull/34678)

## リアルタイム会話開始時のセッションヘッダー追加

リアルタイム会話の開始時にセッションヘッダーが含まれるようになった。

[参考リンク](https://github.com/openai/codex/pull/34681)

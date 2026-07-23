## MCPツールプレフィックスのサーバー別省略設定

サーバーごとに`mcp__`ネームスペースプレフィックスを選択的に除去できるようになった。後方互換性は維持される。

[参考リンク](https://github.com/openai/codex/pull/34991)

## サイドカンバセーションの切り替え操作追加

`toggle_side_conversation`アクション（ctrl-/）が追加され、サイドカンバセーションと親スレッドを閉じることなく切り替えられるようになった。

[参考リンク](https://github.com/openai/codex/pull/35011)

## カスタムプロバイダーのスタンドアロンWeb検索対応

`supports_standalone_web_search`設定が追加され、カスタムプロバイダーが`web.run`ツールを有効化し自身のエンドポイントを通じて検索をルーティングできるようになった。

[参考リンク](https://github.com/openai/codex/pull/34846)

## マルチエージェントWaitツールの無効化設定

マルチエージェントのwait機能を独立して無効化できる設定が追加された。

[参考リンク](https://github.com/openai/codex/pull/34887)

## 信頼済みプラグインスクリプトの帰属管理

検証済みプラグインルートのレジストリが構築され、コマンドを元のプラグインに解決することでプラグインスクリプトを識別・帰属できるようになった。

[参考リンク](https://github.com/openai/codex/pull/35016)

## リモートスキルアイコンURLの公開

スキルインターフェースにnullable な`iconSmallUrl`と`iconLargeUrl`フィールドが追加され、リモートプラグインメタデータから値が設定されるようになった。ローカルスキルではnullとなる。

[参考リンク](https://github.com/openai/codex/pull/35012)

## 更新されたスレッドアイテムのインクリメンタルリプレイ

更新オーディナルが作成オーディナルとは別に追跡されるようになり、更新されたアイテムスナップショットを全体を再処理することなくインクリメンタルに読み取れるようになった。

[参考リンク](https://github.com/openai/codex/pull/35013)

## TUIターン中断のノンブロッキング化

中断リクエストがバックグラウンドで実行される間もスレッドイベントが処理されるようになった。繰り返しの中断は統合され、失敗は警告として表示される。

[参考リンク](https://github.com/openai/codex/pull/35000)

## スキルカタログのコンテキスト予算超過警告

スキルカタログがモデルコンテキスト予算に収まるよう切り詰めまたは説明が短縮された際に警告が発せられるようになった。重複排除も実装された。

[参考リンク](https://github.com/openai/codex/pull/34997)

## MCP接続のランタイムリフレッシュ間での再利用

接続設定が変更されていない場合、MCPランタイム状態のリフレッシュ時に不要なサーバー再起動とツール再リストが回避されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34952)

## 閉じたMCP接続のリコンシリエーション時置換

トランスポートが停止したクライアントの再利用を防ぐ`is_closed`検出が追加され、新しい接続が確保されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34957)

## スレッドMCP状態のMcpRuntimeへの集約

MCP設定、接続、およびルーティングが`McpRuntime`に統合され、モデルステップとツールコール全体で一貫した状態が維持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34930)

## MCPリクエストのデフォルトユーザーエージェント設定

HTTP/OAuthリクエストに`codex-mcp-client/<version>`がデフォルトユーザーエージェントとして送信されるようになった。カスタムヘッダーが優先される。

[参考リンク](https://github.com/openai/codex/pull/34883)

## Codexエラー詳細とリトライメタデータの分離

`CodexErrorDetails`とリトライ遅延が統一`CodexErr`型にラップされ、アナリティクス向けにペイロード不要の`CodexErrKind`分類が生成されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34996)

## 実行環境の最終HTTPポリシーでの初期化

起動サービスがブートストラップデフォルトではなく、設定読み込み後の正しいHTTPポリシー設定を受け取るようになった。

[参考リンク](https://github.com/openai/codex/pull/34995)

## SQLiteホーム設定の全状態コンシューマーへの適用

下流でデータベースパスを再構築する代わりに、`SqliteConfig`がcore/rollout/state/threadレイヤーを通じて受け渡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34994)

## ページネーションスレッドのシングルライター所有権強制

スレッドごとのファイルシステムロックが実装され、一度に1つのアプリサーバープロセスのみがページネーションスレッドに書き込めるようになった。古いロックのクリーンアップも含まれる。

[参考リンク](https://github.com/openai/codex/pull/34986)

## 外部エージェントセッションインポート時のタイムスタンプ保持

インポートされたセッションでインポート時のタイムスタンプではなく、元の時系列メタデータが保持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34989)

## Sleepツールのコードモード外への維持

`clock.sleep`が`DirectModelOnly`としてマークされ、コードモードセッションで直接呼び出し可能だがネストされたツールサーフェスには表示されなくなった。

[参考リンク](https://github.com/openai/codex/pull/34969)

## ローカルマーケットプレースパスの`@`文字対応

ローカルパス構文ではGit ref解析をスキップすることで、相対ローカルマーケットプレースパス内の`@`シンボルが正しく処理されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34959)

## セッションデフォルトの設定バッチ書き込み時の静的維持

モデル/パーソナリティのみの設定のバッチ書き込みがセッションリロードをトリガーせず、永続的デフォルトとして扱われるようになった。

[参考リンク](https://github.com/openai/codex/pull/34940)

## Amazon Bedrock向けAPIプラグインマーケットプレースの使用

BedrockがプロバイダーのときにCodex認証なしで動作できるよう、「openai-api-curated」マーケットプレースが選択されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34931)

## スタンドアロンインストーラーのダウンロード元変更

シェル/PowerShellインストーラーがGitHub Releasesではなく`releases.openai.com`からデフォルトでダウンロードするようになった。フォールバックメカニズムも備える。

[参考リンク](https://github.com/openai/codex/pull/34910)

## ルート認識HTTPクライアントのリダイレクト無効化対応

リダイレクト追跡を無効にするよう設定されたクライアントが、自動的にリダイレクト先を追跡するのではなく初期リダイレクトレスポンスを返すようになった。

[参考リンク](https://github.com/openai/codex/pull/34978)

## スリープ中スレッドのキュー済みエージェントメールでの起床

永続的スリープ状態のアイドルスレッドが、明示的な`trigger_turn`なしでもメールボックスにエージェント作業が到着した際に再開されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34852)

## Freeプランアカウントの画像生成無効化

無料プランユーザーの認証時に画像生成ツールの登録がスキップされるようになった。

[参考リンク](https://github.com/openai/codex/pull/34850)

## リモートプラグインカタログのスコープ別キャッシュ

リモートプラグインカタログ（global/user/workspaceスコープ）のディスクベースキャッシュが実装された。3時間のTTLとバックグラウンドのstale-refreshを備える。

[参考リンク](https://github.com/openai/codex/pull/34849)

## Guardianモデルのレビューセッション制限適用

Guardianがレビュー用に異なるモデルを選択した際、コンテキストウィンドウ/トークン制限のオーバーライドがクリアされ、そのモデル自体の制限が適用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34847)

## バンドルClaude Codeプラグインマーケットプレースの推定

マーケットプレースソースが存在しない場合、`claude-code-plugins`からの有効化プラグインが`anthropics/claude-code`由来として自動帰属されるようになった。

[参考リンク](https://github.com/openai/codex/pull/34979)

## プラグインアプリサマリーのバッチメタデータ使用

プラグインread/installレスポンスのアプリメタデータが認証済みバッチAPI（100件バッチ）を通じて読み込まれるようになった。新しいステータスフィールドも追加された。

[参考リンク](https://github.com/openai/codex/pull/34851)

## ローカルプラグインキャッシュリフレッシュの待機

プラグインリストエンドポイントが、強制リフレッシュ時にローカルキャッシュのリコンシリエーション完了を待ってから結果を返すようになった。

[参考リンク](https://github.com/openai/codex/pull/34877)

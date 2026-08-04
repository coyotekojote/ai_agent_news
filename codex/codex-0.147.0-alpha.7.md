## コマンド承認後の権限再注入の回避

承認済みコマンドプレフィックスを個別に追跡し、exec-policyの修正後に新たに承認されたプレフィックスのみを発行するようになった。

[参考リンク](https://github.com/openai/codex/pull/36800)

## オーディオ準備のユーティリティクレートへの分離

オーディオ入力の正規化とトークン使用量推定のための`codex-utils-audio`ワークスペースクレートが追加された。

[参考リンク](https://github.com/openai/codex/pull/36807)

## ローカルセッションアーカイブコマンドでのSQLite名の優先

ローカルアーカイブ/削除/アーカイブ解除のターゲットがSQLiteから先に解決され、フォールバックスキャンに移行するようになった。

[参考リンク](https://github.com/openai/codex/pull/36808)

## `exec resume --last`でのステートデータベースの優先

再開ルックアップでステートデータベースが最初にクエリされ、ロールアウトのスキャンにフォールバックするようになった。

[参考リンク](https://github.com/openai/codex/pull/36809)

## MCPクライアント適合性リグレッションゲートの追加

Codexをピン留めされたMCPクライアント適合性スイートに対して実行するハーネスが追加された。

[参考リンク](https://github.com/openai/codex/pull/36810)

## 環境ごとのログインシェルポリシーの尊重

ターン環境ごとに有効な`allow_login_shell`設定が保存されるようになった。

[参考リンク](https://github.com/openai/codex/pull/36811)

## コードモード用デュアルWebSocketトランスポートの追加

オプションのデュアルWebSocket機能をネゴシエートし、コールバックをバルクソケット経由でルーティングする機能が追加された。

[参考リンク](https://github.com/openai/codex/pull/36812)

## トークン予算コンテキストでのエージェント名による識別

コンテキストメタデータでスレッドIDの代わりにセッションの正規エージェントパスが使用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/36815)

## 承認リゾルバー名のタイプミス修正

`resolve_tool_apporval`が`resolve_tool_approval`にリネームされた。

[参考リンク](https://github.com/openai/codex/pull/36822)

## 承認テレメトリーコンテキストの統合

`ApprovalCtx`にツール名が追加され、冗長なパラメータが削除された。

[参考リンク](https://github.com/openai/codex/pull/36825)

## コードモードのホストリクエストタイムアウト

`wait`および`terminate`リクエストに60秒のトランスポート猶予が追加された。

[参考リンク](https://github.com/openai/codex/pull/36830)

## Ghosttyでのキーリリースイベント要求の回避

TERM変数によりGhosttyが検出され、キーボード拡張フラグが省略されるようになった。

[参考リンク](https://github.com/openai/codex/pull/36834)

## StatsigエクスポートからのAPIリクエストメトリクス除外

APIリクエストメトリクスがStatsigエクスポーターではランタイム専用として扱われるようになった。

[参考リンク](https://github.com/openai/codex/pull/36840)

## フリーフォームツールの遅延ロードサポート

Responses APIツール定義にオプションの`defer_loading`サポートが追加された。

[参考リンク](https://github.com/openai/codex/pull/36856)

## ネームスペースでのカスタムツールサポート

ネームスペースツール仕様にカスタムフリーフォームツールを含められるようになった。

[参考リンク](https://github.com/openai/codex/pull/36857)

## スレッド生成のリクエストオブジェクトへの統合

`ThreadSpawnRequest`が追加され、スレッドオプションの取り扱いが集約された。

[参考リンク](https://github.com/openai/codex/pull/36862)

## R2アセットパブリッシングのDotSlashによる並列化

アセットアップロードがDotSlashパブリケーションと並行してステージングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/36871)

## スキル拡張機能へのスキルバンドルロードの移行

事前発見されたエグゼキュータースキルバンドルの解析がスキル拡張機能に移行された。

[参考リンク](https://github.com/openai/codex/pull/36877)

## スキル拡張機能への直接スキルディスカバリの移行

直接ロードされたスキルの拡張機能所有のディスカバリが追加された。

[参考リンク](https://github.com/openai/codex/pull/36880)

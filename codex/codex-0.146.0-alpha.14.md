## MCP 2026クライアントサポートの完了

MCP 2026仕様のクライアントサポートが完了した。2026-07-28のディスカバリーサポートも追加された。

[参考リンク](https://github.com/openai/codex/pull/35725)

## WebRTCサイドバンドのRealtime APIルーティング

WebRTCのサイドバンド接続がRealtime APIにルーティングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/35830)

## v2サブエージェントへの開発者インストラクション設定

v2サブエージェントに対してカスタム開発者インストラクションを設定できるようになった。

[参考リンク](https://github.com/openai/codex/pull/35708)

## スレッド整理のためのセクション永続化

スレッドを整理するためのセクション機能が追加され、永続化されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35722)

## Business ProLiteアカウントのセルフサーブ対応

セルフサーブ型のBusiness ProLiteアカウントがサポートされるようになった。

[参考リンク](https://github.com/openai/codex/pull/35785)

## スレッドタイトルの並列読み込み

セッション起動時にスレッドタイトルが並列で読み込まれるようになり、起動パフォーマンスが向上した。

[参考リンク](https://github.com/openai/codex/pull/35779)

## MCPツールカタログの並列解決

MCPツールカタログが並列で解決されるようになり、パフォーマンスが改善された。

[参考リンク](https://github.com/openai/codex/pull/35777)

## レポートへのモデル・エフォート情報の付与

レポートに選択されたターンのモデルとエフォート情報がタグ付けされるようになった。

[参考リンク](https://github.com/openai/codex/pull/35802)

## MCP OAuthの共有HTTPクライアント利用

MCP OAuthリクエストが設定済みの共有HTTPクライアント経由でルーティングされるようになった。TUIネットワークチェックやアナウンスメントの取得にも共有HTTPクライアントが使用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35814)

## スキルメタデータバジェットのコンテキストウィンドウ連動

スキルメタデータのバジェットがコンテキストウィンドウサイズに応じてスケーリングされるようになった。ホストとエグゼキューターのカタログ間でバジェットが共有される。

[参考リンク](https://github.com/openai/codex/pull/35773)

## SQLite接続管理の一元化

SQLite接続の作成が一元化され、ログクライアントでも設定されたSQLiteホームが使用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35828)

## オプショナルMCP起動によるターンブロッキングの回避

オプションのMCPサーバー起動がターンの進行をブロックしないようになった。

[参考リンク](https://github.com/openai/codex/pull/35742)

## ネストされたCodexリクエストの親ターン追跡

ネストされたCodexリクエストにおいて親ターンが追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35835)

## エージェントレジストリのID一貫性確保

エージェントレジストリにおけるIDの一貫性が維持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/35744)

## rmcp 3.0.0-beta.3へのアップグレード

rmcpが3.0.0-beta.3にアップグレードされた。

[参考リンク](https://github.com/openai/codex/pull/35720)

## rusty_v8 150.4.0へのアップデート

rusty_v8が150.4.0にアップデートされた。

[参考リンク](https://github.com/openai/codex/pull/35831)

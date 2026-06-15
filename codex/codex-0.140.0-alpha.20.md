## SQLiteのWALリセットバージョン固定

バンドルされたSQLiteをWALリセット修正済みバージョンに固定し、依存関係更新時に破損バグのあるバージョンにダウングレードされることを防止した。

[参考リンク](https://github.com/openai/codex/pull/27992)

## クロスプラットフォームパス処理の改善

`PathConvention`と`NativePathString`が導入され、プラットフォーム間でネイティブパスを正しくレンダリングできるようになった。

[参考リンク](https://github.com/openai/codex/pull/27819)

## exec-serverのリモート環境cwd・シェル対応

exec-serverがリモート環境のcwdとシェルを尊重するようになった。cwdが`AbsolutePathBuf`から`PathUri`に変換された。

[参考リンク](https://github.com/openai/codex/pull/28122)

## スレッドの親フィルタリング

`thread/list`エンドポイントに実験的な`parentThreadId`フィルタが追加され、スポーンされた子スレッドのクエリが可能になった。

[参考リンク](https://github.com/openai/codex/pull/26662)

## 選択プラグインのMCPカタログ優先順位

選択されたプラグインに対してカタログティアの順序付けが確立され、自動検出と明示的設定の間に位置するようになった。

[参考リンク](https://github.com/openai/codex/pull/27884)

## 選択エグゼキュータープラグインからのstdio MCPサーバー検出

選択されたプラグインの`.mcp.json`をエグゼキューターファイルシステム経由で読み取れるようになった。

[参考リンク](https://github.com/openai/codex/pull/27870)

## マルチエージェントv2プロンプトの更新

デフォルトヒントが協調・委任パターンに合わせて調整された。

[参考リンク](https://github.com/openai/codex/pull/28283)

## プラグインアプリのコネクターリスト保持

ChatGPT/SIWCユーザー向けにプラグイン提供アプリの可視性が維持されるようになった。

[参考リンク](https://github.com/openai/codex/pull/27602)

## プラグインMCP OAuthのスキップ

認証モードに基づいてインストール時にプラグインMCPサーバーがフィルタリングされるようになった。

[参考リンク](https://github.com/openai/codex/pull/27461)

## app-serverでの選択エグゼキュータープラグインMCP有効化

app-serverが選択されたプラグインのstdio MCPを初期化・起動するようになった。

[参考リンク](https://github.com/openai/codex/pull/27893)

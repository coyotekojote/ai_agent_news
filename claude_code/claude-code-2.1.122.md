## `ANTHROPIC_BEDROCK_SERVICE_TIER` 環境変数の追加

Bedrock サービスティア（`default`、`flex`、`priority`）を選択する `ANTHROPIC_BEDROCK_SERVICE_TIER` 環境変数が追加された。`X-Amzn-Bedrock-Service-Tier` ヘッダーとして送信される。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## `/resume` 検索ボックスでの PR URL 貼り付け対応

`/resume` 検索ボックスに PR URL を貼り付けると、その PR を作成したセッションが検索されるようになった。GitHub、GitHub Enterprise、GitLab、Bitbucket に対応。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## `/mcp` で非表示の claude.ai コネクタを表示

手動追加したサーバーと同じ URL を持つ claude.ai コネクタが `/mcp` に表示されるようになり、重複を削除するヒントが表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## OpenTelemetry の改善

- `api_request`/`api_error` ログイベントの数値属性が文字列ではなく数値として出力されるようになった
- `@` メンション解決用の `claude_code.at_mention` ログイベントが追加された

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## `/mcp` の未認可メッセージの明確化

ブラウザサインインフロー後に MCP サーバーがまだ未認可の場合に表示されるメッセージがより分かりやすくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## バグ修正

- 巻き戻されたタイムラインのエントリを含むソースセッションから `/branch` でフォークすると「tool_use ids were found without tool_result blocks」エラーが発生する問題が修正された
- Bedrock アプリケーション推論プロファイル ARN で `/model` に Effort オプションが表示されず、`output_config.effort` が送信されない問題が修正された
- Vertex AI / Bedrock でセッションタイトル生成や構造化出力クエリ時に `invalid_request_error: output_config: Extra inputs are not permitted` が返される問題が修正された
- プロキシゲートウェイ背後のユーザーで Vertex AI `count_tokens` エンドポイントが 400 エラーを返す問題が修正された
- `spinnerTipsOverride.excludeDefault` が時間ベースのスピナーヒントを抑制しない問題が修正された
- ノンブロッキングモードでセッション開始後に接続した MCP ツールが ToolSearch に表示されない問題が修正された
- bash モードで `!exit` / `!quit` がシェルコマンドとして実行されず CLI が終了してしまう問題が修正された
- 新しいモデルに送信される画像が正しい最大 2000px ではなく 2576px にリサイズされる問題が修正された
- リモートコントロールセッションのアイドルステータスが毎秒2回再描画され、`tmux -CC` コントロールパイプが溢れてターミナルが停止する問題が修正された
- 古いビュー設定によりアシスタントメッセージが空白で表示される問題が修正された
- `settings.json` 内の不正な hooks エントリがファイル全体を無効化しないように修正された
- ボイスモード: ターミナルが Caps Lock をキーイベントとして配信しないため、Caps Lock にバインドされたキーバインドがエラーを表示するようになった

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.122)

## プロンプトキャッシュ書き込みトークン使用量の追跡

レスポンスの入力トークン詳細から `cache_write_tokens` が解析され、トークン使用量の集計に反映されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33454)

## 外部エージェント移行の独立クレート化

外部エージェントの検出・インポート・モデル・レポーティングが `codex-app-server` から `codex-external-agent-migration` クレートに移行された。

[参考リンク](https://github.com/openai/codex/pull/33456)

## ターン履歴サマリーでのファイナルアンサー使用

`final_answer` フェーズのエージェントメッセージのみがターンサマリー項目として追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33457)

## コードモード画像生成のタイムアウト延長

初回のコードモード画像生成呼び出しに120秒のyieldが設定されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33459)

## 強制rmコマンド検出の強化

制御フロー、変数展開、パイプライン、トラップ、ネストされたシェル内のリテラルな強制 `rm` が検出されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33464)

## MCPツール呼び出しメタデータからのテンプレートID削除

MCPツール呼び出し項目とライフサイクルイベントから `template_id` が削除された。

[参考リンク](https://github.com/openai/codex/pull/33467)

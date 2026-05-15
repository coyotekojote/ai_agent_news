## RAGスニペットのローカルログ出力

デバッグ目的でRAGスニペットがローカルログファイルに出力されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260515.g928a311fb)

## エンタープライズゲートウェイの認証情報競合防止

エンタープライズゲートウェイでの認証情報の競合が防止され、オプションのAPIキーがサポートされるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260515.g928a311fb)

## NO_PROXY環境変数のMCPサーバー対応

`NO_PROXY`環境変数がネットワークベースのMCPサーバーで尊重されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260515.g928a311fb)

## バグ修正

NixOSおよび他のディストリビューションでのサンドボックスの権限拒否エラーが解消された。編集ウィンドウ末尾の改行が保持されるようになった。Vertex AIの`hasAccessToPreviewModels`フラグが正しく設定され、攻撃的な404フォールバックが削除された。IPC経由の管理者設定比較が安定化され、再起動ループが防止された。脆弱な依存関係が更新された。ファイル処理中のEISDIRエラーが解消された。ファイル解析エラーにENAMETOOLONGおよびENOTDIR例外が追加された。サンドボックスコンテナのスポーン時にエントリポイントが明示的にクリアされるようになった。プロキシサポート修正のため`https-proxy-agent`が外部化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-nightly.20260515.g928a311fb)

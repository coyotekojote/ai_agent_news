## サンドボックス実行のマネージドプロキシ設定強化

Linuxのbubblewrapサンドボックスでプロキシソケットディレクトリを読み取り可能にし、WS_PROXY/WSS_PROXYをマネージドプロキシブリッジ経由でルーティングするようになった。スコープ外の実行から継承されたプロキシ帰属トークンが削除された。

[参考リンク](https://github.com/openai/codex/pull/34641)

## ログインHTTP構築の`HttpClient`への移行

codex-loginが直接のreqwest依存からHttpClientBuilderを使用するよう移行された。カスタムCA、プロキシ、Cloudflare Cookie、サンドボックス、リクエストロギングのポリシーは維持されている。

[参考リンク](https://github.com/openai/codex/pull/34643)

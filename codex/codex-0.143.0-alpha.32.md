## Rendezvous WebSocketのNagle無効化

RendezvousのWebSocket接続においてNagleアルゴリズムが無効化された。エグゼキューターとハーネスの接続呼び出しサイトで`disable_nagle=true`が渡されるようになり、小さな時間に敏感なリレーおよびJSON-RPCフレームのレイテンシが削減された。

[参考リンク](https://github.com/openai/codex/pull/30269)

## 安全通知の文言更新

TUIのバイオセーフティブロックからTrusted Accessアプリケーションに関する古いテキストが削除され、現在承認されている文言に合わせてUIメッセージが更新された。

[参考リンク](https://github.com/openai/codex/pull/30645)

## WebSocketフルテキストトレースの削除

以前のフィルタリング作業で見落とされていた追加のトレースステートメントが削除された。

[参考リンク](https://github.com/openai/codex/pull/30757)

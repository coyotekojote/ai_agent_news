## セキュリティ強化: issue タイトルのサニタイズと信頼できないコンテキストでのラップ

issueタイトルをサニタイズし、`untrusted_context`でラップする処理が追加された。セキュリティ上のリスクが軽減された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28352)

## モデルフォールバック時のセッションIDローテーション

モデルフォールバック発生時にセッションIDをローテーションすることで、ステートフルなAPIエラーが防止されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28469)

## HTTPS強制による資格情報の平文漏洩防止

`GoogleCredentialsAuthProvider`にHTTPSの強制が適用され、資格情報の平文での漏洩が防止されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28517)

## コンテキスト管理無効時のthought partsフィルタリング

コンテキスト管理が無効の場合に`getHistoryTurns`からthought partsをフィルタリングする処理が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28509)

## issueの自動クローズ前にコメントを投稿

caretaker-triageにおいて、issueを自動クローズする前にコメントを投稿する機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28411)

## vitestのv3.2.4へのアップデート

vitestがv3.2.4にアップデートされ、`package-lock.json`ファイルが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28409)

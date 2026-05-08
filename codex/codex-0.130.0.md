## プラグイン詳細のフック表示とプラグイン共有

プラグイン詳細にバンドルされたフックが表示されるようになり、プラグイン共有でリンクメタデータと発見可能性の制御が公開された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## codex remote-control コマンドの追加

`codex remote-control` がヘッドレスでリモート制御可能な app-server を開始するためのシンプルなエントリポイントとして追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## app-server のスレッドページング

app-server クライアントが unloaded、summary、full の各ターンアイテムビューで大きなスレッドをページングできるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## Bedrock の AWS コンソールログイン認証対応

Bedrock 認証が `aws login` プロファイルからの AWS コンソールログインクレデンシャルを使用できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## view_image の環境解決対応

`view_image` がマルチ環境セッションで選択された環境を通じてファイルを解決できるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## app-server スレッドの設定変更反映修正

ライブの app-server スレッドが再起動なしで設定変更を反映するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## ターン差分の正確性修正

apply-patch 操作（ファイルを変更した部分的な失敗を含む）全体でターン差分が正確に維持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## ThreadStore の改善

ThreadStore を通じたスレッドサマリー、リネーム、リジューム、フォークパスの動作が改善され、ローカルロールアウトパスのないスレッドにも対応した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## リモートコンパクションの修正

リモートコンパクションが v2 ストリームで `response.processed` を正しく出力するようになり、API キーコンパクトリクエストで `service_tier` が送信されなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## Windows サンドボックスのアクセス修正

Windows サンドボックスセットアップでサンドボックスユーザーにデスクトップランタイムバイナリキャッシュへのアクセスが付与されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

## codex exec の表示修正

`codex exec` スタートアップバナーから古い「research preview」の文言が削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.130.0)

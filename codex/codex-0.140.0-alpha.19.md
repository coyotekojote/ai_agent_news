## Windows ARM64パッケージングのx64ランナー移行

Windows ARM64のパッケージングジョブがx64ランナー上で実行されるようになった。パッケージングはビルド済みバイナリのダウンロード・署名・圧縮のみで対象コードの実行を伴わないため、ARM64ハードウェアを実際のコンパイルに温存しつつリリースのクリティカルパスが1分43秒短縮された。

[参考リンク](https://github.com/openai/codex/pull/28001)

## exec-serverのcwdをPathUri型に変更

`ExecParams.cwd`フィールドが`PathUri`型に変更され、クロスOS操作がサポートされるようになった。カレントディレクトリはコアおよびrmcpプロデューサー全体でURI形式のまま保持され、`LocalProcess::start_process`時にのみ`AbsolutePathBuf`に変換される。ネイティブでないcwd URIは起動前に拒否される。

[参考リンク](https://github.com/openai/codex/pull/28032)

## プラグインMCPのApp宣言名による重複排除

ChatGPT/SIWCプラグインの動作が改善され、宣言されたApp名と競合するプラグインMCPサーバーのみが非表示になるようになった。App宣言名はロード済みプラグインメタデータに保持されつつ、公開出力は重複排除される。同一プラグインからの競合しないMCPサーバーは引き続き利用可能。

[参考リンク](https://github.com/openai/codex/pull/27607)

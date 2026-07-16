## no_proxyテストの修正

no_proxyのテストが修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28131)

## VertexベースURLの更新

VertexのベースURLが更新された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28145)

## 機密パスブロックリストの大文字小文字無視とVSCode HITL対応

機密パスのブロックリストが大文字小文字を区別しないように修正され、VSCode HITLが対応された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27966)

## @参照ファイルの防御的パス解決の修正

@参照ファイルの防御的パス解決が修正され、macOSテストも修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28053)

## Cloud Run Webhookインジェスションサービスの実装

Caretaker機能としてCloud Run Webhookインジェスションサービスが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28015)

## メモリインポートプロセッサのシンボリックリンクディレクトリエスケープ解決

メモリインポートプロセッサにおけるシンボリックリンクによるディレクトリエスケープの問題が解決された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28233)

## Caretaker Egressサービスのスケルトン実装

Caretaker EgressのCloud Runサービススケルトンが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28167)

## macOSサンドボックスでの~/.gitconfig読み取り専用化

macOSサンドボックスで `~/.gitconfig` が読み取り専用になるように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28221)

## モダンモデル向け文字列リテラルのエスケープシーケンス保持

モダンモデル向けに文字列リテラル内のエスケープシーケンスが保持されるように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28299)

## スクラブされた履歴ターンからのthought除去とthought漏洩の解決

スクラブされた履歴ターンからthoughtが除去され、thought漏洩の問題が解決された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/27971)

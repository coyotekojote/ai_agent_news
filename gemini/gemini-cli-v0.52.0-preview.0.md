## 一時的なCI設定ファイルのワークスペースコンテキスト除外

一時的なCI設定ファイルがワークスペースコンテキストから除外されるようリファクタリングされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28216)

## Caretaker Triageワーカーの基盤モジュール追加

Caretaker Triageワーカーのコア基盤モジュールが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28163)

## Caretaker Egressサービスの GitHub Actionハンドラー実装

Caretaker EgressサービスにOctokit GitHub Actionハンドラーが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28303)

## JSONおよびIPYNBファイルのLLM補正バイパス

`write_file` と `replace` でJSONおよびIPYNBファイルに対するLLM補正がバイパスされるように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28223)

## フォールバックサマリーの前回意図ラベル改善

フォールバックサマリーで曖昧さのない前回意図ラベルが使用されるように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28343)

## Caretaker Triageメインワーカー実行ループの実装

Caretaker Triageのメインワーカー実行ループとEgressアクションパブリッシャーが実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28306)

## Code Assistティアなしアカウントのメッセージ表示

Code Assistティアを持たないアカウントに対して明確なメッセージが表示されるように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28304)

## 共有プロジェクトクォータ制限エラーのセットアップヒント付与

共有プロジェクトのクォータ制限エラーにセットアップヒントが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28391)

## A2Aサーバーのタスクキャンセル時実行ループ中断

A2Aサーバーでタスクのキャンセルが実行ループを確実に中断するように修正された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28316)

## プランモードの書き込みポリシー簡素化

プランモードの書き込みポリシーが相対パスをサポートするよう簡素化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28398)

## google-auth-libraryのバージョンアップ

Node.js向け `google-auth-library` のバージョンが10.9.0にアップグレードされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/28385)

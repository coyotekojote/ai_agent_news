## ワークスペース信頼の強制とタスク分離によるRCE防止

A2Aサーバーにワークスペース信頼の強制とタスク分離保護が追加され、リモートコード実行（RCE）の脆弱性が防止された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## LLMトリアージオーケストレーターの実装

Caretaker-triageサービスにLLMベースのトリアージオーケストレーターとコンテナビルド機能が実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## 無限ReActループおよびプロンプトインジェクションの緩和

ReActループにおける無限ループとプロンプトインジェクションの脆弱性に対する緩和策が実装された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## ツールレスポンスグループ化による400エラー防止

キャンセルされたツールレスポンスをグループ化し、連続するロールを統合することで「400 Bad Request」エラーが防止されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## macOSセキュリティプロファイルのdeny-defaultモデルへの移行

許容的なSeatbeltプロファイルがdeny-defaultセキュリティモデルに再整合され、保護が強化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## 資格情報検証シーケンスの復元

キャッシュされた資格情報の順次チェックと`GOOGLE_APPLICATION_CREDENTIALS`フォールバックメカニズムが復元された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

## evalカバレッジレポートコマンドの追加

テストおよび品質保証ワークフロー向けのevalカバレッジレポートコマンドが導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.53.0)

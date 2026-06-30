## リモートプラグインのデフォルト有効化

リモートプラグインがデフォルトで有効になった。従来のオプトイン方式からオプトアウト方式に変更され、`features.remote_plugin`設定で無効化が可能。

[参考リンク](https://github.com/openai/codex/pull/30297)

## 推論エフォート「max」のファーストクラス対応

`ReasoningEffort::Max`が正式なenum値として追加された。従来は不透明な`Custom("max")`文字列として扱われていたが、Bedrock GPT-5.6カタログとの整合性のためファーストクラスの値となった。UIの大文字表記の不一致も修正された。

[参考リンク](https://github.com/openai/codex/pull/30467)

## モデルメタデータによるスキル使用手順の制御

モデル定義に`include_skills_usage_instructions`メタデータフィールドが導入された（gpt-5.5で有効）。ハードコードされたレガシーモデルマッチングに代わり、メタデータ駆動のアプローチでスキル使用手順の表示を制御する。

[参考リンク](https://github.com/openai/codex/pull/29740)

## v1デリゲーションガイダンスの復元

サブエージェント生成に関する制約が復元された。深掘りやリサーチリクエストにおいて、ローカルで処理する作業とデリゲートする作業の区分が明確化された。

[参考リンク](https://github.com/openai/codex/pull/30511)

## 安全性バッファリングプロンプトのクリア修正

成功したターン後にTUIに残存していた古いモーダルビューが正しくクリアされるようになった。リトライメッセージも更新された。

[参考リンク](https://github.com/openai/codex/pull/30490)

## 自動レビューのプロアクティブプロンプト変更のリバート

自動レビューのオンリクエストプロンプトをよりプロアクティブにする変更（PR #26496）がリバートされた。

[参考リンク](https://github.com/openai/codex/pull/30508)

## 安全性チェックリンクの更新

Bio/Cyberセーフティ関連のURLが更新され、バッファリングUIに欠落していたヘルプセンターリンクが追加された。

[参考リンク](https://github.com/openai/codex/pull/30491)

## AWS Bedrock課題の自動ラベル設定

プロバイダー固有の課題レポートに`aws-bedrock`ラベルを自動適用するラベラーが設定された。

[参考リンク](https://github.com/openai/codex/pull/30607)

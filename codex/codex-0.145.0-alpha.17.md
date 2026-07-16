## rawResponseスキーマへのキャッシュ書き込みトークン追加

`rawResponse/completed` JSONスキーマの使用量内訳に `cacheWriteInputTokens` が追加された。

[参考リンク](https://github.com/openai/codex/pull/33500)

## MCPツール出力の暗号化コンテンツ保持

暗号化メタデータ付きのMCPテキストコンテンツが `encrypted_content` 関数呼び出し出力項目に変換されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33509)

## マルチエージェント設定の統合

エージェント設定が統一された `agents` 設定に集約され、新しい並行性制限とデフォルト値が導入された。

[参考リンク](https://github.com/openai/codex/pull/33550)

## ロール設定時のみのスポーンエージェントタイプ公開

`agent_type` 引数の表示がロールが設定されているシナリオに限定された。

[参考リンク](https://github.com/openai/codex/pull/33572)

## シャドウスキル選択へのフィールドBM25追加

複数フィールドにわたる重み付き重要度を持つ有界BM25セレクターランキングが実装された。

[参考リンク](https://github.com/openai/codex/pull/33605)

## 文字n-gramスキル選択の追加

フィールド重みと逆文書頻度を持つ文字n-gramベースのスキルスコアリングが追加された。

[参考リンク](https://github.com/openai/codex/pull/33613)

## マルチクエリ語彙スキル選択の追加

複合クエリを分割し、クロスビュー候補をマージする語彙セレクターが追加された。

[参考リンク](https://github.com/openai/codex/pull/33614)

## スポーンエージェントの設定済みモデルデフォルト適用

サブエージェントのモデルとreasoning effortに設定済みデフォルトが適用されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33631)

## 生成デフォルトファイルシステムパスバリアントの削除

ファイルシステムポリシーとWindowsサンドボックスの処理が簡素化された。

[参考リンク](https://github.com/openai/codex/pull/33632)

## 起動中環境の待機条件の明確化

環境起動時の待機条件に関するモデルガイダンスが明確化された。

[参考リンク](https://github.com/openai/codex/pull/33633)

## 実行環境分離のガイダンス追加

遅延リクエストの重複排除を含む実行環境の分離に関する開発者ガイダンスが追加された。

[参考リンク](https://github.com/openai/codex/pull/33636)

## 未使用リアルタイムWebRTCクレートの削除

`codex-realtime-webrtc` がCargoワークスペースから削除された。

[参考リンク](https://github.com/openai/codex/pull/33639)

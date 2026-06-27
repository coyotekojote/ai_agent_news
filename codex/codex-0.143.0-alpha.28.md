## npmマーケットプレイスプラグインソースのサポート

マーケットプレイスエントリを通じてnpmレジストリからプラグインをインストールできるようになった。`{"source":"npm", ...}`エントリによりパッケージ名、オプションのバージョン範囲、オプションのHTTPSレジストリ設定をサポートする。`npm pack --ignore-scripts`を使用してスクリプト実行なしでパッケージを取得する。

[参考リンク](https://github.com/openai/codex/pull/29375)

## GPT-5.6のBedrock対応

Amazon BedrockのスタティックモデルカタログにGPT-5.6のSol、Terra、Lunaバリアントが追加された。Bedrock限定の`max`推論エフォートパラメータも導入された。

[参考リンク](https://github.com/openai/codex/pull/30285)

## AGENTS.mdとスキルによる委任認可

`AGENTS.md`ファイルとスキルがマルチエージェントシステムにおける委任をより明示的に認可できるようになった。

[参考リンク](https://github.com/openai/codex/pull/30274)

## ユーザーレベルのコードレビュースキル参照

`$code-review`スキル使用時に、リポジトリレベルだけでなく`$CODEX_HOME/skills/code-review-*`に保存されたユーザーレベルのコードレビュースキルも参照するようになった。

[参考リンク](https://github.com/openai/codex/pull/30143)

## ネストされたMCP認証起動エラーの分類

トランスポートエラー内にネストされた認証必須エラーを検出し、保存されたOAuth資格情報の期限切れ時に`failureReason: "reauthenticationRequired"`と再接続アクションが表示されるようになった。

[参考リンク](https://github.com/openai/codex/pull/30257)

## カスタムツールコールのネームスペース保持

カスタムツールコールで名前空間情報がリクエスト-レスポンスのライフサイクル全体を通じて保持されるようになった。複数の名前空間に同名のツールがある場合の誤ルーティングが修正された。

[参考リンク](https://github.com/openai/codex/pull/30302)

## hooks.jsonのトップレベルメタデータバリデーション緩和

`hooks.json`設定ファイルでトップレベルの`description`文字列フィールドが許可されるようになった。不明なトップレベルキーに対する厳密なバリデーションは維持される。

[参考リンク](https://github.com/openai/codex/pull/30229)

## リモートコントロールのトークンリフレッシュリトライストーム修正

トークンリフレッシュ操作時の一時的なサーバーエラーによるリトライの連鎖的な失敗が修正された。プロアクティブリフレッシュと必須リフレッシュを区別し、サーバー権限ごとのスロットリングを実装した。

[参考リンク](https://github.com/openai/codex/pull/30201)

## セキュリティチェック文言の更新

セキュリティ関連チェックの文言が更新された。生物学研究向けの安全アクセスブロックに関するメッセージと、Trusted Accessリンクが更新された。

[参考リンク](https://github.com/openai/codex/pull/30317)

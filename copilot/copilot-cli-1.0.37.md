## ロケーションベースの権限永続化がデフォルト有効化

同一ディレクトリでの承認がセッション間で引き継がれる、ロケーションベースの権限永続化がデフォルトで有効になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

## `copilot completion` サブコマンドの追加

`copilot completion <bash|zsh|fish>` コマンドが追加され、サブコマンド、フラグ、既知の選択値に対する静的シェル補完スクリプトを生成できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

## セッションピッカーのソート順サイクル

セッションピッカーで `s` キーを押すことでソート順を関連性、最終使用日時、作成日時、名前の間でサイクルできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

## ACP モデル設定の説明・メタデータ

ACP モデル設定オプションに configOptions API を使用するクライアント向けの説明とメタデータが含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

## `/ask` での Markdown レンダリング

`/ask` のレスポンスがテーブルやフォーマット済みリンクを含む Markdown で描画されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

## バグ修正

- 同じモデルまたはエフォートレベルを再選択した場合にモデル・エフォート変更通知が表示されなくなった
- Linux でクリップボード書き込み時に X11 ハンドルがリークする問題が修正された
- 保留中メッセージインジケーターがプロンプトフレームと共に正しく表示されるようになった
- `git branch --show-current` への切り替え後、デタッチド HEAD 検出が常に false を返す問題が修正された
- スキルピッカーでスキルにエラーや警告がある場合にリストが完全に表示されるよう修正された

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.37)

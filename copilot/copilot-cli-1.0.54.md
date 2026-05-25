## セッションの作業ディレクトリ復元

セッションが保存された作業ディレクトリで再開されるようになった。`-C`フラグでオーバーライドが可能。相対パスを値に取るフラグ（`--attachment`、`--log-dir`など）は保存されたcwdから解決される。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## セッション継続時のgitコンテキスト更新

`copilot --continue`でセッションの保存ディレクトリから再開した際に、保存されたブランチとgitコンテキストが古いまま残らず更新されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## コンテキストウィンドウのティア選択の適用

コンテキストウィンドウのティア選択（デフォルト約200K vs 1Mトークン）がエンドツーエンドで適用されるようになり、ティアの選択がコンパクション、トランケーション、トークン表示に正しく反映されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## コマンド安全フィルターの改善

killコマンドの安全フィルターが`kill -0 <PID> 2>/dev/null`のようなシェルリダイレクションを含む有効なコマンドを拒否しなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## AI Credits使用量表示の修正

Responses APIを使用したセッション後にAI Creditsの使用量が正しく表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## レンダリングの改善

tmuxをCygwinまたはminttyで使用する際のレンダリングのスタッターが解消された。スラッシュコマンドピッカーで行が選択されていても(experimental)および(staff)ラベルがオレンジ色で維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## 推論トークン表示の改善

トークン使用量サマリーにおいて、推論トークンが出力トークン数の括弧内に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.54)

## コードモードでのWeb検索サポート

コードモードでスタンドアロンのWeb検索を直接呼び出せるようになった。ネストされたJavaScriptツールコールからの呼び出しにも対応し、プレーンテキストの検索結果を受け取れるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## スキーマ構造の保持強化

ツールおよびコネクタの入力スキーマで`oneOf`および`allOf`構造が維持されるようになった。大規模スキーマのコンパクション時に浅い構造が保持され、MCPツールの互換性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## codex doctorの改善

`codex doctor`ユーティリティでエディタやページャの環境設定詳細が表示されるようになった。JSON出力では機密値が編集される。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## プラグインマーケットプレイスの改善

`codex plugin marketplace list --json`にマーケットプレイスソース情報が含まれるようになった。プラグインリストがバックグラウンドリフレッシュ前にキャッシュされたリモートカタログから返せるようになり、応答性が向上した。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## resume/forkコマンドのパース修正

`codex resume --last`および`codex fork --last`の末尾引数がセッションIDではなく初期プロンプトとして正しく扱われるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## MCP起動時警告のスコープ修正

サブエージェントからの警告がスレッドスコープに制限され、親スレッドの重複アラートやTUIスピナーの停滞が解消された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## 画像編集のターゲット修正

画像編集が会話履歴からの推測ではなく、正確に参照されたファイルパスを使用するようになり、意図した入力に編集が適用されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## URLリンク化の改善

パスにチルダを含むベアURLがTUIで特殊文字の前で切り詰められずに完全にリンク化されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## スレッドリセット時のクラウド設定保持

`/new`、`/clear`、`/fork`などのコマンドが、TUI設定リロード中にクラウド管理の要件やフィーチャーフラグを破棄しなくなった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## サンドボックス実行の改善

サンドボックスが承認済みのエスカレーション決定を一貫して保持し、設定済みのプロキシ専用ネットワーキングを強制するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

## V8ツールチェインの更新

組み込みV8ツールチェインが`rusty_v8`バージョン149.2.0にアップグレードされた。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.139.0)

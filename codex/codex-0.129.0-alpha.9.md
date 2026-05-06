## セッション MCP 設定のリフレッシュ時保持

セッション MCP 設定がリフレッシュ時に保持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## 動的ツール識別子の Responses API 整合

app-server の動的ツール識別子が Responses API と整合された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## プラグイン共有アクセス制御

プラグインの共有アクセス制御が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## プラグインマニフェストキーワードの公開

プラグインマニフェストのキーワードが app-server で公開されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## MCP ターンメタデータにモデルと reasoning effort 追加

MCP ターンメタデータにモデルと reasoning effort が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## スレッド命名の app-server 移行

スレッド命名が app-server に移行された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## Linux スタンドアロン bwrap のバンドル

Linux リリースにスタンドアロンの bwrap がバンドルされるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## V8 サンドボックスの有効化

ソースビルドで V8 サンドボックスが有効化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## TUI セッションピッカーの再設計

TUI のセッションピッカーが再設計された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## クラウドエグゼキュータの登録

exec-server にクラウドエグゼキュータの登録が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## コアレビューフォークの ThreadStore 使用

コアレビューフォークが ThreadStore の履歴を使用するようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## Xcode 26.4 クライアントの MCP elicitation 自動拒否

Xcode 26.4 クライアントに対する MCP elicitation が自動的に拒否されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## レガシー ListSkills/ListModels オペレーションの削除

レガシーの `ListSkills` および `ListModels` オペレーションが削除された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

## バグ修正

- bwrap で libcap がスタンドアロンアーカイブ後に出力されるよう修正された
- MCP で Accept が早期にフィードバックに従って返されるようになった
- Windows Git safe-command ロジックが共有化された
- スレッド分析の `thread_source` が再構築された
- v2 API 定義がモジュールに分割された
- TUI ターンアイテムビューのフィクスチャが修正された
- ツールハンドラがツール名ごとに分割された
- Linux サンドボックスの合成マウントレジストリがユーザーごとに分離された
- bwrap ビルド失敗時のパニックが回避されるようになった

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.129.0-alpha.9)

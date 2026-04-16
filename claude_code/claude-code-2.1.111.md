## Claude Opus 4.7 xhigh の提供開始

Claude Opus 4.7 xhigh が利用可能になった。`/effort` でスピードとインテリジェンスのバランスを調整できる。Opus 4.7 では `high` と `max` の間に位置する `xhigh` エフォートレベルが追加され、`/effort`、`--effort`、モデルピッカーから選択可能。他のモデルでは `high` にフォールバックする。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Max サブスクライバー向け Auto モード

Opus 4.7 使用時、Max サブスクライバー向けに Auto モードが利用可能になった。`--enable-auto-mode` フラグは不要になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/ultrareview` による包括的コードレビュー

クラウド上で並列マルチエージェント分析・批評を行う包括的コードレビュー機能 `/ultrareview` が追加された。引数なしで現在のブランチをレビューするか、`/ultrareview <PR#>` で特定の GitHub PR を取得してレビューできる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/effort` のインタラクティブスライダー

`/effort` を引数なしで実行すると、矢印キーでレベル間を移動し Enter で確定するインタラクティブスライダーが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターミナルテーマ自動マッチ

ターミナルのダーク／ライトモードに自動的に合わせる「Auto (match terminal)」テーマオプションが追加された。`/theme` から選択可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/less-permission-prompts` スキル

トランスクリプトをスキャンして、一般的な読み取り専用の Bash および MCP ツール呼び出しを検出し、`.claude/settings.json` への許可リストを提案する `/less-permission-prompts` スキルが追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windows PowerShell ツールの展開

Windows で PowerShell ツールが段階的にロールアウトされている。`CLAUDE_CODE_USE_POWERSHELL_TOOL` でオプトイン／アウト可能。Linux・macOS では `CLAUDE_CODE_USE_POWERSHELL_TOOL=1` で有効化できる（PATH 上に `pwsh` が必要）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/setup-vertex` と `/setup-bedrock` の改善

`CLAUDE_CONFIG_DIR` 設定時に実際の `settings.json` パスを表示し、再実行時に既存のピンからモデル候補をシードし、対応モデルで「1M コンテキスト付き」オプションを提供するよう改善された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## `/skills` のトークン数ソート

`/skills` メニューで推定トークン数によるソートが可能になった。`t` キーでトグルできる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## その他の改善・修正

- グロブパターン付きの読み取り専用 bash コマンド（例: `ls *.ts`）や `cd <project-dir> &&` で始まるコマンドが許可プロンプトを出さなくなった
- `claude <word>` でタイプミス時に最も近いサブコマンドを提案するようになった
- プランファイルがプロンプトに基づいた名前（例: `fix-auth-race-snug-otter.md`）で作成されるようになった
- `Ctrl+U` が入力バッファ全体をクリアするよう変更された（`Ctrl+Y` で復元可能）
- iTerm2 + tmux 環境での端末表示の乱れが修正された
- `@` ファイルサジェストが非 git ディレクトリで毎ターン全プロジェクトを再スキャンする問題が修正された
- Bedrock/Vertex/Foundry での 429 レートリミットエラーが status.claude.com を参照していた問題が修正された
- Windows 環境で `CLAUDE_ENV_FILE` とセッションスタートフック環境ファイルが正しく適用されるようになった

[参考リンク](https://code.claude.com/docs/en/changelog)

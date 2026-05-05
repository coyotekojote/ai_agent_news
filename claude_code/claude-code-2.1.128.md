## /color コマンドのランダムカラー対応

引数なしで `/color` を実行すると、セッションカラーがランダムに選ばれるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## /mcp のツール数表示

`/mcp` が接続中のサーバーのツール数を表示し、ツール数が 0 のサーバーにフラグを立てるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## --plugin-dir の ZIP アーカイブ対応

`--plugin-dir` がディレクトリに加えて `.zip` プラグインアーカイブも受け付けるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## --channels のコンソール認証対応

`--channels` がコンソール（API キー）認証で動作するようになった。マネージド設定を持つコンソール org は `channelsEnabled: true` の設定が必要。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## モデルピッカーの更新

重複する Opus 4.7 エントリが折りたたまれ、現在の Opus が「Opus 4.7」ではなく「Opus」と表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## OTEL 環境変数の継承停止

サブプロセス（Bash、フック、MCP、LSP）が `OTEL_*` 環境変数を継承しなくなり、OTEL 計装済みアプリが CLI の OTLP エンドポイントを誤って使用する問題が解消された。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## MCP の workspace 予約名

`workspace` が MCP の予約サーバー名となり、既存の同名サーバーは警告付きでスキップされるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## MCP 再接続時のツール一覧簡略化

MCP サーバーの再接続時にツール名の完全一覧でチャットが溢れなくなり、サーバープレフィックスごとにサマリー表示されるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## SDK Bash パーミッションの提案

SDK ホストが Bash パーミッションプロンプトに対して `.claude/settings.local.json` に書き込む永続的な `localSettings` 提案を受け取るようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## EnterWorktree のブランチ作成改善

`EnterWorktree` が `origin/<default-branch>` ではなくローカル HEAD から新しいブランチを作成するようになり、プッシュされていないコミットが失われなくなった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## オートモード分類エラーのヒント表示

オートモードの分類器がアクションを評価できない場合、リトライ、`/compact`、`--debug` での実行といったヒントがエラーに含まれるようになった。

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

## バグ修正

- フォーカスモードで新しいプロンプト送信時に前回の応答が一瞬暗くなる問題が修正された
- Kitty 等のターミナルで `/exit` のたびに「4;0;」デスクトップ通知が表示される問題が修正された
- Remote Control でレート制限時に空の「Opening your options…」メッセージが表示される問題が修正された
- ドラッグ＆ドロップ画像アップロードで画像読み取り失敗時に「Pasting text…」でハングする問題が修正された
- `claude -p` に 10MB 超の入力をパイプした際のクラッシュループが修正された
- フルスクリーンモードで長い URL が各折り返し行で個別にクリックできない問題が修正された
- `--plugin-dir` 経由で読み込んだプラグインで「Marketplace 'inline' not found」と表示される問題が修正された
- MCP ツール結果でサーバーが構造化コンテンツとコンテンツブロックの両方を返した際に画像がドロップされる問題が修正された
- リスト項目内のフェンスコードブロックのコピー時に先頭の空白が含まれる問題が修正された
- `/config` のタブナビゲーションでフォーカスが迷子になる問題が修正された
- OSC 8 ハイパーリンク非対応ターミナルで Markdown リンクのラベルが失われる問題が修正され、`label (url)` 形式で表示されるようになった
- 1M コンテキストモデルで autocompact ウィンドウが小さい場合に「Prompt is too long」で誤ブロックされる問題が修正された
- 並行シェルツールコールで読み取り専用コマンドの失敗が兄弟コールをキャンセルする問題が修正された
- effort をサポートしないモデルでバナーに「with X effort」と表示される問題が修正された
- 3P プロバイダで `/fast` が無関係なスキルにファジーマッチする問題が修正された
- Bedrock デフォルトモデルがリージョン適切なプレフィックスではなく `global.*` に解決される問題が修正された
- vim モード: NORMAL モードの `Space` がカーソルを右に移動するよう修正された（標準 vi/vim の動作）
- ターミナルプログレスインジケーター（OSC 9;4）がツールコール間でちらつく問題が修正された
- `/rename` を引数なしで実行時にコンパクト境界が最終エントリの場合に失敗する問題が修正された
- `--resume`/`--continue` 後に前セッションの「remote-control is active」ステータスラインが残る問題が修正された
- 古い `installed_plugins.json` エントリが PATH を汚染する問題が修正された
- `CLAUDE_CODE_SHELL_PREFIX` にスペースやシェルメタ文字が含まれる場合に MCP stdio サーバーが破損した引数を受け取る問題が修正された
- サブエージェントのプログレスサマリーでプロンプトキャッシュが欠落する問題が修正された（`cache_creation` 約 3 倍削減）
- `/plugin update` が npm ソースプラグインの新バージョンを検出しない問題が修正された
- トランスクリプトが静的な状態でサブエージェントサマリーが繰り返し発火する問題が修正された
- `--output-format stream-json`: `init.plugin_errors` に `--plugin-dir` のロード失敗が含まれるようになった

[参考リンク](https://github.com/anthropics/claude-code/releases/tag/v2.1.128)

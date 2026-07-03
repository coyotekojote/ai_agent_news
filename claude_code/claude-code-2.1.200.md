## AskUserQuestionの自動続行デフォルト無効化

`AskUserQuestion`ダイアログがデフォルトで自動続行しなくなった。`/config`からアイドルタイムアウトをオプトインで設定できる。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## パーミッションモードの名称変更

「default」パーミッションモードがCLI、`--help`、VS Code、JetBrains全体で「Manual」に名称変更された。`--permission-mode manual`および`"defaultMode": "manual"`が`default`と並んで受け付けられる。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## .claude.jsonの非配列値によるクラッシュ修正

`.claude.json`の`disabledMcpServers`または`enabledMcpServers`が非配列値に設定されている場合に起動時クラッシュする問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## バックグラウンドセッションのスリープ/ウェイク後停止修正

スリープ/ウェイク後やストールしたセッションの再開時にバックグラウンドセッションがターン途中でサイレントに停止する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## キャンセルされたターンの再実行防止

Escでキャンセルされたターンがストールリスポーン後にバックグラウンドセッションで再実行される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## daemon.lockのPID再利用問題修正

クラッシュにより残された古い`daemon.lock`のPIDがOSに再利用された場合にバックグラウンドエージェントが二度と起動しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## バックグラウンドエージェントデーモンのハンドオーバー修正

再インストールされた古いビルドがデーモンを乗っ取れないように、ビルドの新しさがバージョンの埋め込みビルドタイムスタンプで判定されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## バックグラウンドエージェントロスターの問題修正

一時的な破損がオーファンクリーンアップを永久に無効化する問題、古いバイナリが新しいバージョンで書き込まれたフィールドを保持しない問題、デーモン再起動時にソケット認証トークンが削除される問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## レートリミットで切断されたサブエージェントの空結果修正

レートリミットによりテキスト出力を生成する前に切断されたサブエージェントが空の結果を返す問題が修正され、クリーンに失敗するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## バックグラウンドエージェント出力の制御バイト修正

バックグラウンドエージェントの出力からの制御バイトがエージェントビューのターミナルに到達する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## claude agents --plugin-dirのフラグ位置修正

`claude agents --plugin-dir <dir>`で`agents`の後にフラグを配置した場合にプラグインのエージェントとスキルがエージェントビューに表示されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## gitワークツリーからのプラグイン読み込み修正

同一リポジトリのgitワークツリーからプロジェクトスコープのプラグインが正しく読み込まれない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## /mcpのスクリーンリーダー対応修正

`/mcp`サーバーリストがスクリーンリーダーとマグニファイアのフォーカスを追跡していない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## 音声ディクテーションのエラーメッセージ改善

録音でオーディオがキャプチャされなかった場合に音声ディクテーションが誤解を招く「Voice connection failed」メッセージを表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## tmux 3.4+でのレンダリングフリッカー修正

同期ターミナル出力を有効にすることでtmux 3.4+でのレンダリングフリッカーが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## スクリーンリーダー出力の改善

装飾グリフが非表示になり、トランスクリプトシンボルが短いラベルとして読み上げられ、ネストされたテーブルが`Header: value.`形式の行として読み上げられるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## インストールスクリプトのメモリ不足説明追加

システムのメモリ不足によりインストールが強制終了された場合に説明が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog#2.1.200)

## ツール承認処理のSession集約

権限フック、レビュアールーティング、承認キャッシュ、ユーザー承認リクエストがセッションレベルの承認フローに集約された。

[参考リンク](https://github.com/openai/codex/pull/37128)

## WindowsパスURI比較のASCII大文字小文字非区別化

`PathUri`の等価比較とハッシュがWindowsドライブおよびUNCパスのASCII大文字小文字を無視するように更新された。

[参考リンク](https://github.com/openai/codex/pull/37129)

## マネージド認証要件のローカル適用

ログイン方法とChatGPTワークスペースのローカル許可リストが追加され、集中ポリシーチェックが実装された。

[参考リンク](https://github.com/openai/codex/pull/37132)

## プロンプト画像リサイズのモデルへの報告

画像リサイズの詳細を報告するデベロッパーメッセージを追加するオプション機能が導入された。

[参考リンク](https://github.com/openai/codex/pull/37134)

## シンボリックリンクされたスキルの検出パス保持

読み込まれた各スキルの検出パスが正規のアイデンティティとともに追跡されるようになった。

[参考リンク](https://github.com/openai/codex/pull/37144)

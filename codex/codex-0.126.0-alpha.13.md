## マイグレーション済みフックパス書き換えの修正

マイグレーションされたフックのパス書き換えが正しく動作しない問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/20144)

## multi-agent v2 が agents.max_depth を無視するよう変更

multi-agent v2 が `agents.max_depth` 設定を無視するように変更された。

[参考リンク](https://github.com/openai/codex/pull/20180)

## 一時停止されたゴールの `/goal resume` 対応

一時停止されたゴールに対して `/goal resume` が使用できるようになった。

[参考リンク](https://github.com/openai/codex/pull/20082)

## Windows 疑似コンソール属性のサンドボックス PTY セッション修正

Windows の疑似コンソール属性ハンドリングがサンドボックス PTY セッションで正しく処理されるよう修正された。

[参考リンク](https://github.com/openai/codex/pull/20042)

## PTYリサイズのクラッシュ耐性強化

PTYリサイズ操作がネイティブクラッシュに対して強化された。リサイズ前にプロセスの生存確認を行うことで、レースコンディションによるクラッシュが防止されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.45.0-nightly.20260529.gc82e2b597)

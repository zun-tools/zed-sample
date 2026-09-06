# Zed入門② — Claude Agent の持ち込みの再現サンプル

動画「【Zed入門②】手持ちの Claude を、サブスクごと持ち込めた」（ずんだもんの実験道具箱）で使ったサンプルです。

## 使い方

```
git clone https://github.com/zun-tools/zed-sample.git
cd zed-sample/no02
zed .
```

1. コマンドパレットで `zed: acp registry` → `Claude Agent` を Install。
2. Agent Panel の「＋」から `New Claude Agent Thread`。
3. 入力欄で `/login` → `Claude Subscription` を選んでブラウザで認可（Claude のサブスクが要ります）。
4. 次の1行を貼って送ると、パネルの中に diff が出ます。`Yes` を押すまでファイルは変わりません。

```
calc.py の div に、ゼロ除算の時に ValueError を投げる処理と docstring を足して
```

`CLAUDE.md` の「日本語の docstring」の指示が効くのを確かめる題材です。

実測: 2026-09-05〜06・Zed 1.18.1・Claude Agent 0.75.1・1テイク。取得のタイミングや認可の挙動は版で変わります。

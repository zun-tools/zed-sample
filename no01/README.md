# Zed入門① — 診断とタスクの再現サンプル

動画「【Zed入門①】Python の拡張なしで開いたら、診断もタスクも居た」（ずんだもんの実験道具箱）で使ったサンプルです。

## 使い方（要るのは Python 3 と Zed だけ）

```
git clone https://github.com/zun-tools/zed-sample.git
cd zed-sample/no01
zed .
```

1. 初めて開くフォルダなので `Unrecognized Project / Restricted Mode` のダイアログが出ます。`Trust and Continue` を押します。
2. `main.py` を開いて待つと、Python 用の拡張を入れていなくても診断が出ます（Ruff と basedpyright を Zed が自分で取ってきます）。
3. コマンドパレットで `task: spawn` → `run sample` を実行すると `hello` が出ます。

`main.py` の未使用変数と綴り違い（`totl`）はわざと入れてあります。

実測: 2026-09-05・Zed 1.18.1・macOS・1テイク。ほかの言語は確かめていません。

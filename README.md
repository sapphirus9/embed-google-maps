# embed-google-maps
**Google マップの共有から「地図を埋め込む」で発行できるHTMLコードを、レスポンシブデザインで使うための1ラインコードです。**<br>
※divで囲っているので、正確には1ラインとは言えないかもしれませんが …

## コード
```
<div class="embed-google-maps" style="position: relative; height: 0; padding-bottom: 80%; overflow: hidden;"><iframe src="｛iframe内のURL｝" width="100%" height="100%" frameborder="0" style="border:0; position: absolute; top: 0; left: 0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe></div>
```

## 使い方
1. Google マップ ⇒ 埋め込み対象の地図を表示 ⇒ 共有 ⇒ 地図を埋め込む ⇒ HTML内のURLをコピー
2. 上記のコードのsrc="`｛iframe内のURL｝`"の箇所をコピーしたURLに置き換え
3. 埋め込みたい箇所にすべてをペーストして完了です
---
- `div class="embed-google-maps"`内にある`padding-bottom: 80%`を変更することで高さを調整することができます
- divにクラス指定はとくに必要ありませんが、把握しやすくするために入れています
- 処理的にはdivで箱を用意して、その中にiframeのGoogle マップをabsoluteで箱いっぱいに配置する形となります

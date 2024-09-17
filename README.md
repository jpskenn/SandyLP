# SandyLP（サンディ エルピー）

![SandyLP keyboard](/assets/README/aaa.jpeg)  

`SandyLP` is a 40% keyboard with symmetrical row staggered layout and key height optimization.

Layered PCB will make height differences for each key.
This covers the lack of optimization to physical key layout in two dimensions that only adjust x-y plane.

---

`SandyLP`は、スイッチの配置を立体的にして高さ方向への最適化を加えた、左右対称ロースタッガード配列の40%キーボードです。  

平面上のキーレイアウトだけでは最適化しきれない部分を、キーの位置に応じてスイッチを配置する高さを変えることで補っています。

[Sandy](https://github.com/jpskenn/Sandy)を元に、ロープロファイルスイッチへの対応と、レイアウトの調整をおこなっています。

名前の由来は、立体的、つまり3Dという意味を込めたSandyの`ロープロファイル版 = Low Profile version`ということで`LP`をつけました。

## 特徴

- 左右対称のキーレイアウト  
  [Jones](https://github.com/jpskenn/Jones)と同様の、2行目と3行目にずれのない、左右対称な、シンメトリカル ロースタッガードのレイアウトです。
  ![左右対称のキーレイアウト](/assets/README/aaa.jpeg)

- キースイッチを立体的に配置  
  3段階の高さで、キースイッチを立体的に配置しています。
  ![キースイッチの高さ](/assets/README/aaa.jpeg)

  平面上のキー配置だけでは最適化しきれない部分を、キーの位置に応じて高さを変え、立体的に配置することで補っています。  

- ロープロファイルのスイッチに対応
  `Choc V2`スイッチに対応（※）し、キーボードの高さを低くおさえることができます。  
  ※`Choc V1`スイッチは、固定ピンを切り取れば使用可能。

- [Remap](https://remap-keys.app)や[VIA](https://www.caniusevia.com)によるキー割り当て変更  
  プログラミング等の知識がなくても、ブラウザ上で簡単にキー割り当てを変更することができます。

- オプション機能  
  以下のオプション機能を使用できます。

  - ロータリーエンコーダ
  - インジケータLED
  - スピーカー

## レイアウト

[![Keyboard Layout Editor: SandyLP](/assets/README/layout.png)  
Keyboard Layout Editor: SandyLP](https://www.keyboard-layout-editor.com/#/gists/29f5da09ffa69ab85efa4c68b556282b)

### キーの高さ

キーの高さはLow（0mm）, Middle（3.6mm）, High（8.6mm）の3段階で、以下のように配置されます。  
![キーの高さ](/assets/README/layout_height_map.png)

### 推奨キーマッピング

設計者の私が使用しているキーマッピングは以下のとおりです。  
[Keyboard Layout Editor: SandyLP](http://)

左右の手の運指を同じにするため、[SemiErgo Layout](https://github.com/mtei/SemiErgo_Layout)に準ずるキーマッピングで使用することを念頭に設計しています。

また、左右端に`Shift`を用意していないので、スペースキーを`Space and Shift`として使用するなど、工夫してください。

## ビルドガイド

- 最新版
  - [SandyLP（DN0010）](/docs/BuildGuide_DN0010.md)

## SNSタグ

[#SandyLP_kbd](https://twitter.com/search?q=%23SandyLP_kbd)

## ギャラリー

準備中

## 参考事例

準備ちゅう

- おおやけハジメさん
- Sparrow

## 開発経緯

元となった`Sandy`を1年半ほど使い続けてきた。  
その体験・経験から得られた情報を実機にフィードバックしたアップデート版（Sandy DN0040）の開発をおこなっていたが、キーボードの高さに対する不満点はロープロファイルスイッチを使用するしか方法がないと判断し、派生版を開発することになった。

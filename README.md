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
  [Jones](https://github.com/jpskenn/Jones)と同様の、2行目と3行目にずれのない、左右対称なシンメトリカル ロースタッガードのレイアウトです。  
  ![左右対称のキーレイアウト](/assets/README/aaa.jpeg)

- キースイッチを立体的に配置  
  [Sandy](https://github.com/jpskenn/Sandy)と同じく、キースイッチを3段階の高さで立体的に配置しています。  
  平面上ではキーを配置できる範囲が限られるため、一部のキーはどうしても指が届きにくくなってしまいます。例えば[Jones](https://github.com/jpskenn/Jones)では、右手小指の`P`や`Back Space`、`Enter`などは打鍵しやすくなりましたが、右手人差し指の`Y`は少し遠く感じられます。  
  このような箇所について、キーの位置に応じてスイッチを配置する高さを変えることで打鍵のしやすさを向上させています。  
  ![キースイッチの高さ](/assets/README/aaa.jpeg)

- ロープロファイルのスイッチに対応  
  `Choc V2`スイッチに対応（※）し、キーボードの高さを低くおさえることができます。  
  パームレストを使わずとも、手首を反らさないポジションで打鍵できます。
  ※`Choc V1`スイッチは、固定ピンを切り取れば使用できます。

- [Remap](https://remap-keys.app)、[Vial]()によるキー割り当ての変更  
  プログラミング等の知識がなくても、キーやロータリーエンコーダの割り当てを、ブラウザ（Remap）を使って簡単に変更できます。  
  また、Vial対応のファームウェアも用意しています。

- オプション機能  
  以下のオプション機能を使用できます。  
  - ロータリーエンコーダ
  - インジケータLED
  - スピーカー

## レイアウト

最下行中央にロータリーエンコーダを取り付けることができます。  
[![Keyboard Layout Editor: SandyLP](/assets/README/layout.png)  
Keyboard Layout Editor: SandyLP](https://www.keyboard-layout-editor.com/#/gists/29f5da09ffa69ab85efa4c68b556282b)

### キーの高さ

キーの高さはLow（0mm）, Middle（3.6mm）, High（8.7mm）の3段階で、以下のように配置されます。  
![キーの高さ](/assets/README/layout_height_map.png)

### 推奨キーマッピング

設計者の私が使用しているキーマッピングは以下のとおりです。  
[Keyboard Layout Editor: SandyLP](http://)

左右の手の運指を同じにするため、[SemiErgo Layout](https://github.com/mtei/SemiErgo_Layout)に準ずるキーマッピングで使用することを念頭に設計しています。

また、左右端にシフトキーを用意していないので、スペースキーを`Space and Shift`として使用するなど、工夫してください。

## ビルドガイド

- 最新版
  - [SandyLP（DN0010）](/docs/BuildGuide_DN0010.md)

## SNSタグ

[#SandyLP_kbd](https://twitter.com/search?q=%23SandyLP_kbd)

## ギャラリー

準備中

## 参考事例

準備中

- おおやけハジメさん
- Sparrow

## 開発経緯

この`SandyLP`の元となった[Sandy](https://github.com/jpskenn/Sandy)を1年半ほど使い続け、長期ロードテストとして十分な体験・経験からの情報を得ることができた。  
その情報を実機にフィードバックしたSandyのアップデート版（Sandy DN0040）の開発をおこない、あとは基板の製造をする段階となっていた。  
しかし、課題のひとつとして挙げていた手首の負荷軽減（＝キーボードを低くする変更）が取り込まれていないことが、様々な思いの中でほんのりと燻っていた。  
ちょうどその頃`Choc V2`スイッチにとても素性の良い静音タイプのスイッチが追加されたことと、「もしかしたら、自分が好んで使っているMX用のキーキャップも使えるかもしれない。」という思いで、ロープロファイルのスイッチを使用したSandy派生版の開発に踏み切った。  

また、使用するスイッチの変更でそこそこの量の設計変更が見込まれることから、ついでにキーレイアウトも変更することにした。  
これまでの`Jones`や`Sandy`では頒布・販売することを念頭に、想定するユーザーの最大公約数的なところへ歩み寄ったレイアウトだったが、今回は自分の使用スタイルを最優先し、自分にとって不要な数字行や左右端のシフトキーなどを取り除いた、少し尖ったレイアウトへと変更した。

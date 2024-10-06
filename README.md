# SandyLP（サンディ エルピー）

![SandyLP keyboard](/assets/Readme/DSCF5282.jpeg)  

`SandyLP` is a 40% keyboard with symmetrical row staggered layout and key height optimization.

Layered PCB will make height differences for each key.
This covers the lack of optimization to physical key layout in two dimensions that only adjust x-y plane.

---

`SandyLP`は、スイッチの配置を立体的にして高さ方向への最適化を加えた、左右対称ロースタッガード配列の40%キーボードです。  

平面上のキーレイアウトだけでは最適化しきれない部分を、キーの位置に応じてスイッチを配置する高さを変えることで補っています。

[Sandy](https://github.com/jpskenn/Sandy)を元に、ロープロファイルスイッチへの対応と、レイアウトの調整をおこなっています。

名前の由来は、立体的、つまり3Dという意味を込めたSandyの`ロープロファイル版 = Low Profile version`ということで`LP`をつけました。

## 特徴

### 左右対称のキーレイアウト  

[Jones](https://github.com/jpskenn/Jones)と同様の、2行目と3行目にずれのない、左右対称なシンメトリカル ロースタッガードのレイアウトです。  
![左右対称のキーレイアウト](/assets/Readme/DSCF5300.jpeg)

一般的なロースタッガードなレイアウトとの共通性を残しつつ、左右対称で打鍵しやすくなるよう、[SemiErgo Layout](https://github.com/mtei/SemiErgo_Layout)に準ずるキーマッピングで使用することを念頭に設計しています。  
Z行の左右端にシフトキーを用意していないので、スペースキーを「Space and Shift」として使うと便利です。

各種キーキャップセットのうち「Base Kit」と呼ばれる基本的なキットですべてを埋めることができます。また、104キーの英語キーキャップセットでも十分実用が可能です。
![左右対称のキーレイアウト](/assets/Readme/layout_for_base_kit.png)

詳しくは、[Keyboard Layout Editor: SandyLP](https://www.keyboard-layout-editor.com/#/gists/29f5da09ffa69ab85efa4c68b556282b)を参照してください。

### キースイッチを立体的に配置  

[Sandy](https://github.com/jpskenn/Sandy)と同じく、キースイッチを3段階の高さで立体的に配置しています。  
平面上ではキーを配置できる範囲が限られるため、一部のキーはどうしても指が届きにくくなってしまいます。例えば[Jones](https://github.com/jpskenn/Jones)では、右手小指の`P`や`Back Space`、`Enter`などは打鍵しやすくなりましたが、右手人差し指の`Y`は少し遠く感じられます。  
このような箇所について、キーの位置に応じてスイッチを配置する高さを変えることで打鍵のしやすさを向上させています。  

![キースイッチの高さ](/assets/Readme/DSCF5294.jpeg)
![キースイッチの高さ](/assets/Readme/DSCF5284.jpeg)
![キースイッチの高さ](/assets/Readme/DSCF5296.jpeg)

キーの高さはLow（0mm）, Middle（3.6mm）, High（8.7mm）の3段階で、以下のように配置されます。  
![キーの高さ](/assets/README/layout_height_map.png)

### ロープロファイルのスイッチに対応  

`Choc V2`スイッチに対応（※）し、キーボードの高さを低くおさえることができます。  
パームレストを使わずとも、手首を反らさないポジションで打鍵できます。
※`Choc V1`スイッチは、固定ピンを切り取れば使用できます。

### Remap、Vialによるキー割り当ての変更  

プログラミング等の知識がなくても、キーやロータリーエンコーダの割り当てを、ブラウザ等を使って簡単に変更できます。  

### オプション機能  

- ロータリーエンコーダ
- インジケータLED
- スピーカー

## ビルドガイド

- 最新版
  - [SandyLP（DN0010）](/docs/BuildGuide_DN0010.md)

## SNSタグ

[#SandyLP_kbd](https://twitter.com/search?q=%23SandyLP_kbd)

## ギャラリー

![SandyLP keyboard](/assets/Readme/DSCF5282.jpeg)  
w/ NuPhy nSA BOW

## 参考事例

- [TreK Lagoon](https://zenn.dev/digitarhythm/articles/a559b4b19fc959) by おおやけハジメ さん
- [Sparrow62](https://github.com/74th/sparrow62-buildguide/blob/master/sparrow62_v2.md) by 74th さん

## 開発経緯

以前開発した[Sandy](https://github.com/jpskenn/Sandy)を1年半ほど使い続け、日常使いの長期ロードテストとして十分な情報を得ることができた。  
その情報を元にSandyのアップデート版（Sandy DN0040）の開発をおこない、あとは基板製造の発注をする段階となっていたが、Sandyの課題のひとつとして挙げていた手首の負荷軽減、つまりキーボードを低くする変更を取り込まなかったことが様々な思いの中でほんのりと燻っていた。

ちょうどその頃、Choc V2スイッチのラインナップに大変素性の良い静音タイプが追加され、自分が好んで使っているMX用のキーキャップもChoc V2で使えそうな情報を得られたことから、ロープロファイルのスイッチを使用したSandyの派生版開発に踏み切った。  

使用するスイッチの変更により、派生版の開発ではそこそこの量の設計変更が見込まれることから、ついでにキーレイアウトも変更することにした。  
これまでの`Jones`や`Sandy`では頒布・販売することを念頭に、想定するユーザーの最大公約数的なところへ歩み寄ったレイアウトだったが、今回は自分の使用スタイルを最優先し、自分にとって不要な数字行や左右端のシフトキーなどを取り除き、少し尖ったレイアウトへと変更した。

こうして、SandyLPが誕生することとなった。
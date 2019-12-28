# キーマップについて考える

##  考えたこと

* スペースキーを小指に割り当てる。

* 修飾キーを親指にする。


## 文字優先順位

* 有名な配列は日本語には合わない。
これは英語と日本語で文字使用頻度が異なるからである。
よって、日本語英語両方の頻度から考える

[文字頻度表](http://www7.plala.or.jp/dvorakjp/hinshutu.htm) を参考に、
各文字ごとの割合を英語と日本語で高い方から選んでいく。

上のリンクの表を日本語英語両方一緒にして割合で降順にソートし、
高い方から2回目に現れた文字を削除した。
よって、下記の表の割合は足しても100%にはならない。
英語を大文字、日本語を小文字にした。

順位  | 各言語での割合 | 文字  |     | 順位  | 各言語での割合 | 文字
:---: | ---:           | :---: | --- | :---: | ---:           | :---:
1     | 12.319%        | a     |     | 14    | 3.728%         | y
2     | 11.749%        | i     |     | 15    | 3.195%         | C
3     | 11.400%        | E     |     | 16    | 2.671%         | M
4     | 10.614%        | o     |     | 17    | 2.140%         | w
5     | 8.884%         | u     |     | 18    | 2.023%         | P
6     | 8.184%         | T     |     | 19    | 1.984%         | F
7     | 7.467%         | n     |     | 20    | 1.858%         | g
8     | 6.973%         | S     |     | 21    | 1.644%         | B
9     | 6.222%         | R     |     | 22    | 1.381%         | z
10    | 5.930%         | k     |     | 23    | 0.998%         | V
11    | 4.255%         | H     |     | 24    | 0.205%         | J
12    | 3.873%         | L     |     | 25    | 0.176%         | X
13    | 3.870%         | D     |     | 26    | 0.083%         | Q


## キーのコスト

よくヒートマップが載せてあるが、実際自分で使って見るとコスト評価と感覚に大きな違いがあった。
いわゆる個人差であろう。
せっかく自分専用に作るのであるから汎用性はこの際無視したい。

下記の表はHelixキーボードを実際にぽちぽちしてみてキーの押しやすさを数値にしてみたものである。
表の縦横の軸は配列単純に左上を基準に0から番号を降ったものである。
あくまで私の主観的な押しやすさに過ぎない。

### やっていてわかったこと

1. 左右の手で同じ指でもコストが違うことがわかった。
* 人差し指と小指は左右の手で押しやすさに違いが大きかった。
	* 左手の小指の性能が意外と高買ったことである。
	逆に右手の小指はポンコツであった。

1. 当たり前ではあるが、ホームポジション上では小指に近いキーであっても、
薬指で押下する方がコストが低いということもあった。
左上のEscapeキーなどは小指を使わず薬指を使う方が圧倒的に押しやすかった。

1. よくあるコスト表ではホームポジションの下の段はそれなりに押しやすいことになっているが、
私にとっては指を曲げるよりは伸ばす方のキーが圧倒的に押しやすかった。

1. ノートパソコンのようにキーボードの周囲がキーの高さと同じものと違い、
独立したキーボードでは左下と右下のキーを指の根本で打鍵しやすかった。

1. 腕とキーボードの角度は打鍵しやすさに大きな影響を与えていた。
Helixキーボードは左右分離型であるため左右で角度を調節できる。
これはかなり都合がよかった。
また、腕と手首の角度のうち手招きする方向の角度についてもかなり影響があった。


| index | 0     | 1     | 2     | 3     | 4     | 5     | 6     | 7     | 8     | 9     | 10    | 11    | 12    | 13    | 14    |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | 9     | 10    | 10    | 10    | 10    | 10    |       |       |       | 10    | 10    | 10    | 10    | 10    | 10    |
| **1** | 5     | 8     | 2     | 2     | 2     | 5     |       |       |       | 4     | 2     | 2     | 2     | 7     | 5     |
| **2** | 4     | 1     | 1     | 1     | 1     | 2     |       |       |       | 2     | 1     | 1     | 1     | 2     | 4     |
| **3** | 7     | 4     | 6     | 6     | 3     | 5     | 11    |       | 4     | 3     | 3     | 7     | 7     | 6     | 7     |
| **4** | 8     | 12    | 12    | 12    | 3     | 1     | 2     |       | 2     | 1     | 3     | 12    | 12    | 9     | 8     |




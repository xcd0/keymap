# キーマップについて考える

##  考えたこと

* スペースキーを小指に割り当てる。

* 修飾キーを親指にする。


## 文字優先順位

* 有名な配列は日本語には合わない。  
これは英語と日本語で文字使用頻度が異なるからである。  
よって、日本語英語両方の頻度から考える。  

[文字頻度表](http://www7.plala.or.jp/dvorakjp/hinshutu.htm) を参考に、
各文字ごとの割合を英語と日本語で高い方から選んでいく。  

上のリンクの表を日本語英語両方一緒にして割合で降順にソートし、  
高い方から2回目に現れた文字を削除した。  
よって、下記の表の割合は足しても100%にはならない。  
英語を大文字、日本語を小文字にした。  
表はあえて一定で区切らず、割合の差が大きなところで区切った。

| 順位  | 文字  | 割合  | 順位   | 文字  | 割合 | 順位   | 文字  | 割合  | 順位   | 文字  | 割合  | 順位   | 文字  | 割合   |
| :---: | :---: | ---:  | :---:  | :---: | ---: | :---:  | :---: | ---:  | :---:  | :---: | ---:  | :---:  | :---: | ---:   |
| **1** | a     | 12.3% | **5** | u     | 8.8% | **11** | H     | 4.2%  | **17** | w     | 2.14% | **21** | B     | 1.64%  |
| **2** | i     | 11.7% | **6** | T     | 8.1% | **12** | L     | 3.8%  | **18** | P     | 2.02% | **22** | z     | 1.38%  |
| **3** | E     | 11.4% | **7** | n     | 7.4% | **13** | D     | 3.8%  | **19** | F     | 1.98% | **23** | V     | 0.99%  |
| **4** | o     | 10.6% | **8** | S     | 6.9% | **14** | y     | 3.72% | **20** | g     | 1.85% | **24** | J     | 0.205% |
|       |       |       | **9** | R     | 6.2% | **15** | C     | 3.19% |        |       |       | **25** | X     | 0.176% |
|       |       |       | **10** | k     | 5.9% | **16** | M     | 2.67% |        |       |       | **26** | Q     | 0.083% |


## キーのコスト

よくヒートマップが載せてあるが、実際自分で使って見るとコスト評価と感覚に大きな違いがあった。  
いわゆる個人差であろう。  
せっかく自分専用に作るのであるから汎用性はこの際無視したい。  

下記の表はHelixキーボードを実際にぽちぽちしてみてキーの押しやすさを数値にしてみたものである。  
表の縦横の軸は配列単純に左上を基準に0から番号を降ったものである。  
あくまで私の主観的な押しやすさに過ぎない。  

| index | 0     | 1     | 2     | 3     | 4     | 5     | 6     |       | 7     | 8     | 9     | 10    | 11    | 12    | 13    |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | 9     | 10    | 10    | 10    | 10    | 10    |       |       |       | 10    | 10    | 10    | 10    | 10    | 10    |
| **1** | 5     | 8     | 2     | 2     | 2     | 5     |       |       |       | 4     | 2     | 2     | 2     | 7     | 5     |
| **2** | 4     | 1     | 1     | 1     | 1     | 2     |       |       |       | 2     | 1     | 1     | 1     | 2     | 4     |
| **3** | 7     | 4     | 6     | 6     | 3     | 5     | 11    |       | 4     | 3     | 3     | 7     | 7     | 6     | 7     |
| **4** | 8     | 12    | 12    | 12    | 3     | 1     | 2     |       | 2     | 1     | 3     | 12    | 12    | 9     | 8     |

### コストについて

単純に集計すると下記のようになる。

| コスト | 左手  | 右手  | 合計  | コスト | 左手  | 右手  | 合計  | コスト | 左手  | 右手  | 合計  |
| :---:  | :---: | :---: | :---: | :---:  | :---: | :---: | :---: | :---:  | :---: | :---: | :---: |
| **1**      | 5     | 4     | 9     | **7**      | 1     | 4     | **5**     | 10     | 5     | 6     | 11    |
| **2**      | 5     | 6     | 11    | **8**      | 2     | 1     | **3**     | 11     | 1     | 0     | 1     |
| **3**      | 2     | 3     | 5     | **9**      | 2     | 1     | **3**     | 12     | 3     | 2     | 5     |















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

1. 単純に距離では近い場合でも位置によってはかなり押しやすさが違った。  
例えば、(0,0)と(0,1)では距離とコストが反転している。  
これは左上角の場合外側に他のキーがないためラフに打鍵しても誤入力になりにくいためであった。



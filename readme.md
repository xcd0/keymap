# キーマップについて考える

##  考えたこと

* スペースキーを小指に割り当てる。

* 修飾キーを親指にする。

* キーごとのコスト評価では左右の手で全然違うということ。

* 有名な配列は日本語には合わない。

## 文字優先順位

日本語英語両方の頻度から考える

http://www7.plala.or.jp/dvorakjp/hinshutu.htm

ここを参考に各文字ごとの割合を英語と日本語で高い方から選んでいく。

上のリンクの表を日本語英語両方一緒にして割合で降順にソートし、
高い方から2回目に現れた文字を削除した。よって、下記の表の割合は足しても100%にはならない。
英語を大文字、日本語を小文字にした。

順位 | 各言語での割合 | 文字
:---: | ---:           | :---:
1    | 12.319%        | a
2    | 11.749%        | i
3    | 11.400%        | E
4    | 10.614%        | o
5    | 8.884%        | u
6    | 8.184%        | T
7    | 7.467%        | n
8    | 6.973%        | S
9    | 6.222%        | R
10   | 5.930%        | k
11   | 4.255%        | H
12   | 3.873%        | L
13   | 3.870%        | D
14   | 3.728%        | y
15   | 3.195%        | C
16   | 2.671%        | M
17   | 2.140%        | w
18   | 2.023%        | P
19   | 1.984%        | F
20   | 1.858%        | g
21   | 1.644%        | B
22   | 1.381%        | z
23   | 0.998%        | V
24   | 0.205%        | J
25   | 0.176%        | X
26   | 0.083%        | Q


## キーのコスト

よくヒートマップが載せてあるが、実際自分で使って見るとコスト評価と感覚に大きな違いがある。
さらに左右の手で同じ指でもコストが違うことがわかった。
また、ホームポジション上では小指に近いキーであっても薬指で押下する方がコストが低いということもあった。
つまりキーのコスト評価は個人差が大きいのであった。



| index | 0     | 1     | 2     | 3     | 4     | 5     | 6     | 7     | 8     | 9     | 10    | 11    | 12    | 13    | 14    |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **0** | 9     | 10    | 10    | 10    | 10    | 10    |       |       |       | 10    | 10    | 10    | 10    | 10    | 10    |
| **1** | 5     | 8     | 2     | 2     | 2     | 5     |       |       |       | 4     | 2     | 2     | 2     | 7     | 5     |
| **2** | 4     | 1     | 1     | 1     | 1     | 2     |       |       |       | 2     | 1     | 1     | 1     | 2     | 4     |
| **3** | 7     | 4     | 6     | 6     | 3     | 5     | 11    |       | 4     | 3     | 3     | 7     | 7     | 6     | 7     |
| **4** | 8     | 12    | 12    | 12    | 3     | 1     | 2     |       | 2     | 1     | 3     | 12    | 12    | 9     | 8     |




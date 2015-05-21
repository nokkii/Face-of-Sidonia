# Face-of-Sidonia
Android Wear Watch face of Sidonia

![Figure1](https://dl.dropboxusercontent.com/u/7009453/IMG_20150302_134558.jpg)
アンビエントモード
![Figure2](https://dl.dropboxusercontent.com/u/7009453/IMG_20150521_113343.jpg)

# 表示の見かた
上の青いステータス部、真ん中の黄色い中央部に分かれています。

### 中央部の見かた
真ん中に黄色の大字で時、分が表示されています。

### ステータス部の見かた
数字を三文字にしたい関係で下二桁は日付ですが、上1桁に1-12月表記の下一桁が
表示される仕様になっています。なので1月と12月、2月と12月の違いがわからない仕様になっています。

### ステータス部時計機能
今はDisableになっていますが、ステータス部に時計を表示する関数があります。
Face上にピークカードを大きく表示すると、分が隠れるのでそういう時に便利です。
下二桁は分ですが、上1桁に0-11時表記の下一桁が表示される仕様になっています。
午前と午後はTの下にAとPで表現されている(AM/PMと書くと時計丸出しでださかった)ので
上のステータス部だけ見ると、1時と11時の違いがわからない仕様になっています。

# 仕様
固定部分のフォントは自分で書きましたが、動的に切り替わる部分のフォントは外部フォントを利用しています。
完成度を上げるなら現在使用している以下の文字に関してまじめにフォントを作成したい。
「TAPS1234567890心圧温能析設通令位 零壱弐参肆伍陸漆捌玖」
あと、中央に大字で時間を表示しているけど原作デザイン的にはアリなのかよく分かっていない。

中央の4文字を管理するCenterPoint, 上部のステータス部を管理するStatus,
Watch fase全体を管理するFaceOfSidoniaクラスで管理されています。

# 外部素材
以下の外部フォントを使用しています

## 漢字
### M+ M1 Regular
Copyright 2002 M+ FONTS PROJECT

## 英数字
### Browning
Copyright 2003 www.liberatorcrew.com

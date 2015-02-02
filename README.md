# cocotile-spec
ココタイル仕様

タイルデータの所在メタデータ「ココタイル」のファイル仕様です。
ココタイルは、地理院地図 http://maps.gsi.go.jp/ の「表示範囲で絞り込み」を実現するために使用されています。

# URL
```
http://cyberjapandata.gsi.go.jp/xyz/cocotile/{z}/{x}/{y}.csv
```
18/239192/93905 （標準地図では http://cyberjapandata.gsi.go.jp/xyz/std/18/239192/93905.png ) のココタイルの URL は http://cyberjapandata.gsi.go.jp/xyz/cocotile/18/239192/93905.csv です。

# ファイル内容
そのタイル位置に存在する（地理院）タイルの {t} がカンマ区切りで羅列されています。
例えば、 http://cyberjapandata.gsi.go.jp/xyz/cocotile/18/239192/93905.csv の内容は次のとおりです。
```csv
std,pale
```
これは、このタイル位置に標準地図（std）と淡色地図（pale）が存在していることを示しています。

# 履歴
2015-02-03 作成

UTAS 「オンライン授業URL」の入力欄に書かれた文字列の処理方法詳細
================================================================

基本
================================================================

* http://...  https://...  の部分を自動的にアンカー <a href="...">...</a> にする
* 改行を &lt;br /&gt; にする

仕様詳細
================================================================

* https://utelecon.github.io/code/anchorize/anchorize.py の 関数 anchorize(s) が仕様の詳細
 * 改行で区切る
 * 各行から http, httpsの正規表現にマッチした部分を取り出す
 * 正規表現はコードを参照 (要詳細議論)
 * 日本語文字はURLとは見なさない  https://abc.com/資料/ は https://abc.com/ までをURLとみなす
 * 「URLはhttps://abc.com/です」  のようなケースで, 「です」を含めないための判断

実行例
================================================================

 * [https://utelecon.github.io/code/anchorize/](https://utelecon.github.io/code/anchorize/) を開いてください
 * p?.txt というのがもともとの文字列, p?.html が処理結果


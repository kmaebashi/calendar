# Calendar
## これは何?
JavaScriptでカレンダーを表示するプログラムです。

## 使い方
Calendarクラスとして提供されています。
```
<script type="text/javascript" src="./calendar.js"></script>
<link rel="stylesheet" type="text/css" href="calendar.css">
(中略)
<div id="calendar"></div> ←カレンダーを貼るdivを用意しておく
(中略)
<script>
const elem = document.getElementById("calendar");
// カレンダーを貼る要素と初期選択の日付を渡して、Calendarを生成する。
const calendar = new Calendar(elem, new Date());
// 日付をクリックしたときにコールバックされるメソッドの設定。
// コールバックされる際、選択された日付をDateオブジェクトで引数で渡される。
calendar.setDatePickedCallback(clicked);
……
// 任意のタイミングで、getCurrentDate()で現在選ばれている日付を取得することも可能。
const date = calendar.getCurrentDate();
</script>
```
詳細はtest.htmlを参照してください。

## ライセンスについて
NYSL Version 0.9982とします。作者は一切の著作権を主張しませんので、改変するなり煮るなり焼くなり好きにしてください。
http://www.kmonos.net/nysl/

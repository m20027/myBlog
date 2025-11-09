---
title: 有用なサイト
layout: page
---

新規タブで開かないので注意
1. [Common and Less Common Magnets and Metals][magnets_metals]
2. 


[magnets_metals]: https://berman-shoenberg.blogspot.com/

<body>
<p>更新日: <time id="modified_date"></time></p>
<script>
/**
  * ステップ1
  * ファイルの更新日を取得
  */
// HTMLファイルの最終更新日を取得
const last = new Date(document.lastModified);
/**
  * ステップ2
  * 取得した日付データを「年・月・日」に分けて取得
  */
  // 取得した日付を「年・月・日」に分けて変数に格納する
const year = last.getFullYear();
const month = last.getMonth() + 1;
const date = last.getDate();
// 月・日の値を修正した後に格納する変数を用意する
let fixedMonth = month;
let fixedDate = date;
/**
  * ステップ4
  * 上書き用の日付のテキストを作成
  */
// 表示用のテキストを作成 例: 2024年2月8日
const viewDateText = year + "年" + month + "月" + date + "日";
// データ用の文字列を作成 例: 2024-02-08
const datetimeText = year + "-" + fixedMonth + "-" + fixedDate;
/**
  * ステップ5
  * HTMLの要素に値を上書き
  */
// 更新日の表示先のHTML要素「time」タグを取得
const target = document.getElementById('modified_date');
// timeタグの内容を上書きする
target.textContent = viewDateText;
</script>
</body> 

# Lecture 1 HTML
## First Layout
```html
<html>
  <head>
    <!--  這邊主要是瀏覽器看的一些設定 -->
  </head>
  <body>
    <!--  這邊主要是給使用者看的內容-->
  Hello HTML!
  </body>
</html>
```

## Title 標題
```html
<html>
  <head>
    <title>First Step to HTML</title>
  </head>
  <body>
  </body>
</html>

```
除了網頁標題
做好一點的網站，會在某個子網頁的標題顯現
子畫面 - 網站
ex: 某某產品 - 某某購物網站
來增加 SEO 的 RANK

## Header and Paragraph 標題和段落
```html
<html>
  <head>
    <title>First Step to HTML</title>
  </head>
  <body>
    <h1>標題</h1>
    <h2>標題</h2>
    <h3>標題</h3>
    <h4>標題</h4>
    <h5>標題</h5>
    <h6>標題</h6>
    <p>aajdoifo ajsdapd foirnv </p>
  </body>
</html>
```
有六種大小的標題

## List 清單
### unorder list
```html
<ul>
  <!-- unorder list -->
  <li>我是一筆清單</li>
  <li>我是一筆清單</li>
  <li>我是一筆清單</li>
  <li>我是一筆清單</li>
  <li>我是一筆清單</li>
</ul>
```
### order list
```html
<ol>
  <!-- order list -->
  <li>有順序的清單</li>
  <li>有順序的清單</li>
  <li>有順序的清單</li>
  <li>有順序的清單</li>
  <li>有順序的清單</li>
</ol>
```

## Tag

```html
<標籤 屬性1="value" 屬性2="value"></標籤>
```

### 粗體
```html
<strong>Lorem</strong> <b>Ipsum</b>
```

**`<strong>` v.s. `<b>`**

`strong`是去強調這個內容，`b`是去讓文字外觀變成粗體(bolic)。

對於可以一般用視覺讓上網的使用者是沒有太大的差異，但是對於用一些視障人士，用聽的來看這個網站時，`strong`會讓讀報軟體聲音變大聲，強調了那個字

另外還有搜尋引擎在搜尋的時候，也會去認這些標籤，來達到辨識語意，知道 `strong` 是要強調的意思。

### 斜體
`<em>` for emphasize, `<i>` for italic
```html
<em>issimply</em>
<i>dummy</i>
```

**`<em>` V.S. `<i>` (italic)**

跟前面的  `strong` 和 `b` 的關係類似，`<em>`比`<i>`更有強調的意思。此外 `<strong>` 的強調度也大於 `<em>`。

在HTML5的標準裡面，這四個標籤都可以用。

## 超連結
`<a>` for `anchor`

```html
<a href="http://google.com">連到Google</a>
```
最簡單的形式

```html
<a href="http://google.com" target="_blank">連到Google</a>
```
會打開新視窗，還是在原本視窗跳到新網站

```html
<a href="http://google.com" target="_blank" title="此標題會開啟新視窗">連到Google</a>
```
title 可以有個小tooltip顯示說這個連結會做什麼事情
target 可以控制說按下這個連結後，是開新視窗還是在原視窗更換

## div and span
`div` for division
比較是分區的概念，會框出一個區塊，span比較是範圍的意思

假設我在段落裡面，想要標記一段文字來做特別效果，通常會使用span，如果使用div，如下
```
<p>
Lorem Ipsum has been the <div>industry's standard</div>dummy text ever since
</p>
```
通常會瀏覽器糾正為
```html
<p>
Lorem Ipsum has been the
</p>
<div>industry's standard</div>
"dummy text ever since"
<p>
</p>
```

## 表格
最簡單3*3表格
```html
<table>
  <caption>我是表格標題</caption>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
</table>
```

簡單地把加上每欄每列的標題
```html
<table>
  <caption>我是表格標題</caption>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
  <tr>
    <td>我是資料</td>
    <td>我是資料</td>
    <td>我是資料</td>
  </tr>
</table>
```

現在有比較仔細劃分表頭跟表內容的方式
```html
<table>
  <caption>我是表格標題</caption>
  <thead>        
    <tr>
      <th>我是標題</th>
      <th>我是標題</th>
      <th>我是標題</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>我是資料</td>
      <td>我是資料</td>
      <td>我是資料</td>
    </tr>
    <tr>
      <td>我是資料</td>
      <td>我是資料</td>
      <td>我是資料</td>
    </tr>
    <tr>
      <td>我是資料</td>
      <td>我是資料</td>
      <td>我是資料</td>
    </tr>
  </tbody>
</table>
```

## 表單
### Label and Input
Label 和 Input 有兩種寫法

第一種，把input包在label裡，通常用在radio 和 checkbox
```html
<div>
  <label>
      女
      <input type="radio" id="female">
  </label>
</div>
```

第二種，input跟label拆開，通常文字欄位會是這個寫法
```html
<div>
  <input type="radio" id="male">
  <label for="male">
      男
  </label>
</div>
```

然後你會發現，明明我們通常是男跟女會擇一，可是若合併上面兩塊（如下），兩個選項卻可以都同時選
```html
<div>
  <label>
    <input type="radio" id="female">
    女
  </label>
</div>
<div>
  <input type="radio" id="male">
  <label for="male">
    男
  </label>
</div>
```

此時為兩者都加上同一個name，就會變成只能選其中一個了
```html
<div>
  <label>
    <input type="radio" name="gender" id="female">
    女
  </label>
</div>
<div>
  <input type="radio" name="gender" id="male">
  <label for="male">
    男
  </label>
</div>
```

### button
button 有兩種寫法，要選擇哪一種，可能就看你後端那邊喜歡怎麼接，或者是在做DOM操作或寫CSS哪個比較方便再挑。(這裡是我暫時查到的說明兩者不同的[文章](http://web.archive.org/web/20110721191046/http://particletree.com/features/rediscovering-the-button-element/
)

```html
<div>
  <input type="button" value="我是按鈕">
</div>
```
```html
<button></button>
```

## Image
```html
<img src="" alt="">
```
`src`是圖片來源，`alt`是圖片掛的時候的替代文字


## TAG 整理
```
標題 h1~h6
內文 p

清單
ul
ol
li
dl 定義清單
dt 標題
dd 內容，描述 dt 這個標題

連結 a

表格
table 表格
thead 表頭
tbody 表內容
tfoot 表尾
tr
th 每一欄或每一列的標題
td
caption 大表格標題

表單（傳統）
form                  表單
lable                 標籤
input type="checkbox" 方塊打勾/複選
input type="radio"    圓圈/單選
input type="text"     單行文字
input type="password" 密碼
input type="button"   按鈕
input type="file"     上傳檔案
textarea              多行文字/留言
select                下拉式選單
  option              選單的選項

擴充HTML5
表單
input type="mail"     郵件(手機上使用時，鍵盤會預設是有@)
input type="tel"      電話(會切換成數字鍵盤)
文章
article               最主要的內容
section               章節
                      上面兩個可以互包，譬如說首頁裡面可以有很
                      多個section放不同的 article，一個長的
                      article也可以裡面放很多section
aside
header                文章前言
footer                
nav                   導覽(整個網站應該只會有一個)
```

emmet快速外掛(3乘3表格):  `table>tr*3>td*3`

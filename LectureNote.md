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
有七種大小的標題

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

#### `<strong>` v.s. `<b>` (bolic)
`strong`是去強調這個內容，`b`是去讓文字外觀變成粗體。

對於可以一般用視覺讓上網的使用者是沒有太大的差異，但是對於用一些視障人士，用聽的來看這個網站時，`strong`會讓讀報軟體聲音變大聲，強調了那個字

另外還有搜尋引擎在搜尋的時候，也會去認這些標籤，來達到辨識語意，知道 `strong` 是要強調的意思。

### 斜體
`<em>` for emphasize, `<i>` for italic
```html
<em>issimply</em>
<i>dummy</i>
```
#### `<em>` V.S. `<i>` (italic)
跟前面的  `strong` 和 `i` 類似，`<em>`比`<i>`更有強調的意思。此外 `<strong>` 的強調度也大於 `<em>`。

在HTML5的標準裡面，這四個標籤都可以用。

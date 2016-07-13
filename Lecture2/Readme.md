# Lecture 2 CSS
CSS Define Guide
## CSS 寫法
```CSS
selector {
  CSS屬性1: 值;
  CSS屬性2: 值;
}
```

## CSS 設定處
### Inline CSS
寫在標籤後面，在style後面直接CSS寫法
```html
<p style="color: #fff;font-size: 30px;">
```
很常在七八年前的dreamweaver上面看到，但是performance最好。
缺點就是非常難以維護。

### 寫在頁首
```html
<html>
  <head>
    <style type="text/css">
      p {
        font-size: 16px;
        color: #00f;
      }
    </style>
  </head>
  <body>
  </body>
</html>
```

## CSS 類型
- 文字
  - 字級 font-size
  - 色彩 color
  - 字體 font-family
    - `font-family: '華康娃娃體', '華康少女體', '水管體', '黑體', '新細明體', san-serif;`
    - 會依序去看說電腦裡有沒有這個字體，沒有的話就往下套
    - 通常會用字型的英文名稱來做設定
    - san-serif 是預設的無襯線字體
  - 斜體 font-style
    - `font-style: italic;`  仿斜體 (用CSS去模擬斜體)
  - 粗體 font-weight
    - Range: 100 ~ 900
    - 100 ~ 300 細, 400 ~ 600 粗, 700 ~ 900 特粗
    - `font-weight: bold;` 仿粗體
  - 裝飾 text-decoration
- 段落
  - 行距 line-height
    - 很少會用固定大小，通常都會根據字體大小
    - 通常黑體字會調行距大，有襯線字會行距小
  - 段落間距 margin （外距）
    - margin 是指外部距離，物件跟物件之間的距離，邊界
  - 留白 padding （內距、墊充）
    - padding 是指物件跟內容物之間的距離
  - 首行縮排 text-indent
    - 通常會用em來做單位，em是指一個字的大小
  - 字距
    - word-spacing 每個單字
    - letter-spacing 每個字母
  - 強迫不換行
- 背景
  - 背景顏色 background-color
  - 背景圖片路徑 background-image
  - 背景圖片重複 background-repeat
    - no-repeat
    - repeat-x
    - repeat-y
  - 背景圖片位置 background-position
    - 有九個點可以使用
  - 背景圖片尺寸 background-size
    - cover 可以使圖片滿版，但是視窗大小移動時，圖片比例不變
    - contain 圖片一定要完完整整的照圖片比例，多出來的部分會就空白
  - 背景圖片固定 background-attachment
    - 背景要不要隨著畫面捲動
    - fix: 固定在背後

## Layout
### Box Model
(看layout-exercise.html)
- 參數
  - Width 物件寬度
  - Padding 物件框和內容物的寬度
  - Margin 物件之間的寬度
  - Border 物件邊緣
- 佔據空間: W+P+B+M
- 可見尺寸: W+P+M

### clear
可以用 `clear: both;`來隔開float效果(看layout-exercise2.html)

#
## CSS Reset
#### meyerweb CSS
讓網頁排版在各個瀏覽器的排版一致，徹底清掉 CSS
http://meyerweb.com/eric/tools/css/reset/

#### Normalize css
把必要的譬如粗體，斜體留著
https://necolas.github.io/normalize.css/

## Block and inline
#### Block 區段
會佔位，會佔掉一整個列，也可設定寬高，
ex: `<ul>`, `<ol>`, `<p>`, `<div>`

#### Inline 區段
不會佔位，不會佔掉一整個列，設定寬高會無效，
ex: `<strong>`, `<img>`, `<a>`

下圖藍色為block，紅色為inline
![](block_inline.png)

## Position
- static 靜態：很少用到
- relative 相對：自身偏移
  - top, left, right, left 等設定是相對於**資料流**的偏移
- absolute 絕對：定位於父層，但又有很多例外設定
  - 找父層有沒有設定定位(relative, absolute, fixed 三種)，如果沒有，就繼續往上找
  - 找到的話，就會靠著那一層做絕對定位
  - 使用這個的話，會讓物件抽離資料流
- fixed 固定：固定於視窗

請看 `demo_position_xxx`系列
## CSS selector
- S `space` B: A 底下所有的 B 物件
- A `>` B: A下一層的 B 物件
- A `+` B: 緊跟在 A 後面的 B
- A `~` B: A 之後的所有物件 B

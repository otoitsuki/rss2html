
# 用 Google Feed API 把 RSS 轉成 HTML 

## 用途

利用 Google Feed API 把任何 RSS 轉成 HTML 就像是 Blog Widget 一樣可以把文章內容插到網頁上任一處。

## 實際Demo

<http://codepen.io/anon/pen/ZOzNWx>

## 使用方法

1. 在要顯示 RSS 內容的地方增加`<div class="article-list"></div>`

2. 修改`rss2html.js`，把要轉成 HTML 的 RSS 貼到 `var rssUrl =""` 引號裡去。  
也可修改 `rssNum` 的數字，決定一次要呈現多少篇文章，預設是 5 篇。

3. 在 html 中插入 jQuery 連結和 js 檔案 

	* jQuery：`<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>`
	* Javascript：`<script src="rss2html.js">`

	建議是放在`</body>`上方。

4. 完成

## 美化頁面
html 架構如下，可以自行設計 CSS 美化頁面。
```
<div class="article-list">
  <div class="article">
    <div class="article-metadata">
      <span class="date"></span>
    </div>
    <div class="article-info">
      <h3 class="title">
        <a href="#"></a>
      </h3>
      <p class="content"></p>
    </div>
  </div>
</div>
```

## License

Copyright (c) 2016 Itsuki.  
See the LICENSE file for license rights and limitations (MIT).

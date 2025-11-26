---
title: Web Frontend Beginner Tutorial
description: 讓你擁有操控 HTML、CSS、JS 的超能力
date: 2025-11-26T11:59:29.317Z
featured_image: /do-something-great.jpg
draft: false
tags:
    - CSS
    - HTML
    - JavaScript
    - Tutorial
    - Beginner
categories:
    - Frontend
    - Web
keywords:
    - CSS
    - Frontend
    - HTML
    - JavaScript
    - Matsuzu
    - Tutorial
    - Beginner
fmContentType: posts
---

歡迎來到前端世界！當我們瀏覽網頁時，無論是查看新聞、購物，還是觀看影片，我們所看到的一切文字、圖片、按鈕、互動效果，都是由三種基礎技術協同工作所產生的。這三位黃金搭檔就是：**HTML (結構)、CSS (樣式) 和 JavaScript (行為)**。

<!--more-->

### HTML：網頁的骨架、血肉 (結構與內容)

**HTML (HyperText Markup Language，超文件標記語言)** 是所有網頁的**基礎**。它不是一種程式語言，而是一種**標記語言**，它使用**標籤 (Tags)** 來標記網頁上的不同內容，告訴瀏覽器這些內容是什麼。

#### 核心概念：標籤 (Tags) 與元素 (Elements)

HTML 文件由一系列的**元素 (Elements)** 組成。一個元素通常由**起始標籤**、**內容**和**結束標籤**構成。

* **標籤範例：**

    * `<p>`：用於標記一個**段落** (Paragraph)。
    * `<h1>`：用於標記最高層級的**標題** (Heading)。
    * `<img>`：用於嵌入**圖片** (Image)。

* **HTML 結構範例：**

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>我的第一個網頁</title>
    </head>
    <body>
        <h1>歡迎來到前端世界</h1>
        <p>這是網頁的內容，我用段落標籤包起來。</p>
        <a href="https://www.google.com">點擊這裡</a>
    </body>
</html>
```

這段程式碼就是一個網頁的**基本骨架**。

**HTML 的職責是：** 確保網頁上的所有內容 (標題、段落、圖片、連結、列表、表格、表單) 都能以**正確的結構**呈現在瀏覽器上。它定義了「這是標題」、「那是圖片」、「這是使用者可以點擊的連結」。

-----

### CSS：網頁的皮膚 (樣式與美化)

如果說 HTML 定義了內容，那麼 **CSS (Cascading Style Sheets，層疊樣式表)** 就是用來**美化和佈局**內容的技術。CSS 讓網頁從純文字的單調文件，變成我們現在看到的豐富多彩、視覺吸引人的介面。

#### 核心概念：選擇器 (Selectors) 與規則 (Rules)

CSS 工作的基本單位是**樣式規則 (Style Rule)**，它由一個**選擇器 (Selector)** 和一個或多個**宣告區塊 (Declaration Block)** 組成。

  * **選擇器：** 告訴 CSS 你想要修改**哪一個**或**哪一組** HTML 元素。

  * **宣告區塊：** 包含了你想要套用的樣式，例如 `property: value;`。

  * **CSS 樣式範例：**

```css
h1 {                    /* 選擇器：選擇所有 <h1> 標籤 */
    color: blue;        /* property: value; 設定文字顏色為藍色 */
    font-size: 32px;    /* 設定字體大小 */
}

p {                     /* 選擇器：選擇所有 <p> 標籤 */
    text-align: center; /* 設定文字置中 */
    margin-top: 20px;   /* 設定上方邊距 */
}
```

**CSS 的職責是：** 決定網頁上元素的**外觀**和**空間佈局**。它負責回答：「標題的字體顏色要是藍色」、「段落要靠左對齊」、「這張圖片要放在網頁的右側」等視覺問題。

近年的 CSS 發展，特別是 **Flexbox (彈性盒子)** 和 **Grid (格線佈局)** 的出現，讓前端工程師能夠更輕鬆、更強大地控制網頁的**響應式佈局 (Responsive Design)**，確保網頁在不同尺寸的設備 (手機、平板、電腦) 上都能優雅地呈現。

-----

### JavaScript (JS)：網頁的靈魂 (行為與互動)

**JavaScript (JS)** 是一種功能強大的**程式語言**。它是讓網頁從靜態變成**動態**、**可互動**的關鍵。JS 是前端技術中最複雜、最活躍的一部分，它賦予了網頁**生命**。

#### 核心概念：DOM 操作與事件處理

JS 最常做的事情是：

1.  **操作文件物件模型 (DOM, Document Object Model)：**
    DOM 是瀏覽器將 HTML 文件解析後建立的一棵「樹狀結構」。JS 透過 DOM 介面，可以**動態地新增、移除、修改**網頁上的任何 HTML 元素或 CSS 樣式。

2.  **事件處理 (Event Handling)：**
    JS 可以監聽使用者的各種**事件**，例如：點擊按鈕、滑鼠移動、鍵盤輸入、表單送出等，並在事件發生時執行特定的程式碼。

**JavaScript 互動範例：**

```javascript
// 獲取網頁上 ID 為 'myButton' 的按鈕元素
const button = document.getElementById('myButton');

// 當使用者點擊這個按鈕時，執行函式
button.addEventListener('click', function() {
    // 彈出一個提示框
    alert('你點擊了我！');

    // 也可以改變網頁上的文字內容
    document.getElementById('message').textContent = '內容已被 JavaScript 改變！';
});
```

**JS 的職責是：** 創造**使用者體驗**和**動態行為**。它負責處理：「當使用者點擊這個按鈕時，請彈出一個視窗並改變某處的文字」、「當使用者滾動到頁面底部時，自動載入更多內容」、「在使用者輸入表單資料時，即時檢查資料是否有效」等複雜的互動邏輯。

-----

### 總結：前端開發的黃金三角

| 技術名稱 | 角色比喻 | 主要職責 | 關鍵詞彙 |
| :--- | :--- | :--- | :--- |
| **HTML** | **骨架** | 定義網頁的**結構**和**內容**。 | 標籤、元素、結構、語義化 |
| **CSS** | **皮膚** | 定義網頁的**外觀**和**佈局**。 | 樣式、選擇器、佈局、響應式設計 |
| **JavaScript** | **靈魂** | 處理網頁的**行為**和**互動**邏輯。 | DOM 操作、事件、動態、程式邏輯 |

作為前端新手，你的學習路徑應該是：

1.  **紮實掌握 HTML：** 學習所有核心標籤，理解**語義化** (Semantic HTML) 的重要性。
2.  **專注於 CSS 佈局：** 學會使用 Flexbox 和 Grid，讓你的網頁能夠在各種設備上看起來都很棒。
3.  **開始寫 JS：** 從最基礎的變數、函式開始，接著學習如何操作 DOM 和處理使用者事件。

這三者是不可分割的整體。一個沒有 CSS 的 HTML 是醜陋的；一個沒有 JS 的 HTML 和 CSS 是呆板的；而沒有 HTML 的網頁則根本不存在。

現在，你已經對前端開發的核心技術有了一些的了解。旅程才剛剛開始，但你已經站上了正確的起跑線！
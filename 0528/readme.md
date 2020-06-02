# 響應式網頁 0528 課程綱要

## CSS
### CSS分類
#### 嵌入式樣式
```html
<h1 style="color:red;">Title</h1>
```
#### 內部樣式
```html
<head>
	<title>標題</title>
	<style>
		h1 {
			color: red;
		}
	</style>
</head>
```
#### 外部樣式表
```html
<head>
	<title>標題</title>
	<link rel="stylesheet" href="style.css">
	<style>
		@import url("style.css");
	</style>
</head>
```
### 基本選取器
#### 標籤 tag
```css
p {
	color: red;
}
```
#### 類別 class
使用點開頭命名，可重複使用
```css
.abc {
	color: blue;
}
```
#### ID
使用#開頭，不可重複使用
```css
#xyz {
	color: yellow;
}
```
#### 萬用選取器 * 
預設套用在網頁的所有元素
```css
* {
	font-family: "Segoe UI";
}
```
### CSS 權重
當CSS發生衝突時，CSS會以權重去做區分。CSS影響的範圍愈小，權重就越重，權重越重，優先順序越高。
在預設的狀態下，權重大小：ID > CLASS > TAG
### CSS 文字相關樣式 
#### color --- 文字顏色

>快速鍵 c

```css
h1 {
    color: red;                /*色彩名稱*/
    color: rgb(255,0,0);       /*RGB色碼*/
    color: rgba(255,0,0,.5);   /*RGBA色碼*/
    color: #ff0000;            /*16進位*/
    color: #f00;               /*16進位縮寫*/
    color: hsl(112, 80%, 36%)  /*色相飽和度明度*/
}
```
>16進位算法
rgb(30,0,200)
30 / 16 = 1...14
0 / 16 = 0...0
200 / 16 = 12...8
#商餘商餘商餘
如果遇到十位數就轉換為A，所以16進位的16個分別為
0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F
rgb(30,0,200) => #1E00C8
***
#### text-align --- 文字對齊

>快速鍵:ta

*  left
* center
* right
* justify
***
#### text-decoration --- 文字裝飾

>快速鍵:td

* none
* underline
* overline
* line-through
***
#### font-size --- 字體大小

> 快速鍵:fz
>
單位:
* px
* em
* rem

> em 與 rem 的差別
> em 的比例是依循最靠近的父元素；rem 的比例是依循根的比例。假設父元素是 24px，子元素是 1.6em，最後的大小就是 24 x 1.6；若子元素是1.6rem，則還是維持 16 x 1.6。
***
#### font-family --- 字體種類

>快速鍵:ff
> 
```css
font-family: 字體名稱 ;
```
除了使用預設的字體以外，也可以使用 Google 網路字體(Web Font)。
[Google Fonts](https://fonts.google.com/)
***
#### font-weight --- 粗體字

>快速鍵:fw
* bold
* 100-900
* normal
***
####  font-style --- 斜體字
>快速鍵:fs
> 
* italic
* normal
### 補充網站
* [Color Hung](https://colorhunt.co/)
* [Coolors](https://coolors.co/)
* [Nippon Colors](https://nipponcolors.com/)
* [Google Fonts](https://fonts.google.com/)

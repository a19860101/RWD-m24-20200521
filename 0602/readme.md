# 響應式網頁 0602 課程綱要
## CSS
### CSS文字相關樣式
#### letter-spacing --- 字元間距
>快速鍵:ls
字元之間的距離。
***
#### word-spacing --- 文字間距
>快速鍵:wos
英文單字之間的距離，中文無效
***
#### line-height --- 行高
>快速鍵:lh
行與行之間的距離，文字會在行高的正中間
***
#### text-transform --- 文字變形
文字大小寫。
>快速鍵:tt 
* uppercase
* lowercase
* capitalize
***
#### font-variant --- 小型大寫字母
小型大寫字母
>快速鍵:fv

***
***
### CSS背景相關樣式 
#### background-color背景色

> 快速鍵: bgc
> 
```css
background-color: 色碼 ;
```
#### background-image 背景圖片或漸層

> 快速鍵: bgi
> 
* url() - 圖片
```css
background-image: url("圖片位置") ;
```
* linear-gradient() - 線性漸層
```css
background-image: linear-gradient(to right, red 30%,blue 40%, yellow 50%, green 60% );
```
* repeating-linear-gradient() - 線性重複漸層
```css
background-image: repeating-linear-gradient(45deg,transparent 0px,transparent 10px,blue 10px,blue 20px); 
```
* radial-gradient() - 放射性漸層
```css
background-image: radial-gradient(red 30%,blue 30%,blue 40%,yellow 40%, yellow 50%,green 50% );
```
* repeating-radial-gradient() - 放射性重複漸層
```css

```
***
#### background-repeat背景的重複方式

> 快速鍵: bgr
> 
* repeat - 完全重複
* repeat-x - x軸重複
* repeat-y - y軸重複
* no-repeat - 不重複

```css
background-repeat: repeat ;
```
***
#### background-position背景的位置

> 快速鍵: bgp
> 
```css
background-position: 100px 50px ;
/*背景水平偏移100px，垂直偏移50px*/
```
除了用數值表示，也可以使用方位
* top
* bottom
* center
* left
* right
```css
background-position: right top;
/*背景靠右上*/
```
***
#### background-attachment背景固定方式

> 快速鍵: bga
> 
* scroll - 捲動
* fixed - 固定

```css
background-attachment: fixed ;
```
***
#### background-size背景的大小

>快速鍵: bgz
> 
* contain - 等比例符合內容
* cover - 等比例填滿內容
***
***
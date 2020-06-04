# 響應式網頁 0604 課程綱要
## CSS
### 排版相關
#### width ---寬度
元素寬度
#### height--- 高度
元素高度。
> 若要讓高度可以滿版，有以下兩種做法
```css
/*作法一*/
html,body {
	height: 100%;
}
.box {
	height: 100%;
}
/*作法二*/
.box {
	height: 100vh;
}
```
#### 群組選取器
```css
html, body {
    height: 100%;
}
/* 同時選取html與body標籤 */
```
***

#### border--- 邊框
```css
border:color style width;/*順序可交換*/
border-left: color style width;
border-right: color style width;
border-top: color style width;
border-bottom: color style width;

border-left:color style width;
border-right:color style width;
border-top:color style width;
border-bottom:color style width;

border-left-color: color;
border-right-color: color;
border-top-color: color;
border-bottom-color: color;

border-left-width: width;
border-right-width: width;
border-top-width:width;
border-bottom-width: width;

border-left-style:style;
border-right-style:style;
border-top-style:style;
border-bottom-style:style;
```
可使用的樣式-style
* solid
* double
* dotted
* dashed
* inset
* outset
* groove
* ridge

***
#### padding ---內距
邊框到內容之間的距離
* padding-left
* padding-right
* padding-top
* padding-bottom
* padding
***
#### margin--- 外距
邊框以外到下一個元素之間的距離
* margin-left
* margin-right
* margin-top
* margin-bottom
* margin
***
#### 縮寫(僅margin、padding有效):
在margin與padding中可使用縮寫的方式設定不同位置的距離。

```css
margin:10px;                /*上下左右*/
margin:10px 30px;           /*上下10px,左右30px*/
margin:10px 30px 0px;       /*上10px,左右30px,下0px*/
margin:10px 30px 0px 20px;  /*上10px,右30px,下0px,左20px*/
```
***
#### block與inline的差異
##### block
1. block永遠都會往下換行，如果有設定寬度，右方空缺的部分會由margin自動填滿；如果沒有設定寬度，則寬度會視為100%
2. 在block元素中，width、height、margin、padding、border都有作用
##### inline
1. 內容有多少，範圍就有多少
2. width、height、margin-top、margin-bottom沒有作用
3. padding-top、padding-bottom、border-top、border-bottom看的見效果，但不影響實際空間

> 基本上只要是行內元素，就不建議使用width,height,border,margin,padding這些屬性，如果要使用就轉換成block或是inline-block之類的其他模式
> 
#### display --- 轉換元素
* block
* inline
* inline-block
* table
* table-cell
* table-row
* flex
* inline-flex
* grid 

#### box-sizing
元素在預設的狀態時，總寬度=width+border+padding、總高度=height+border+padding，設定box-sizing之後不管padding與border設定多少，寬度依然保持原始的值
```css
* {
    box-sizing: border-box;
}
```
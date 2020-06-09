# 響應式網頁 0609 課程綱要

## CSS
### CSS排版相關

#### 區塊置中
預設狀態下，區塊右邊剩餘的空間都是margin，預設為margin-right: auto，在這邊auto可以視為自動填滿margin；若將margin-left設定為auto時，則變成左邊填滿，區塊就會移到右邊；左右同時設定auto，區塊就會置中。

#### calc  運算
如果是有數值的屬性，皆可使用calc()做計算
```css
.container {
    width: calc(100% / 3);
    height: calc(100px + 50px);
}
```
> 在運算子的前後要加上空格，否則會造成解析錯誤
#### float
文繞圖。讓區塊靠左或靠右浮動。
>在float下方的區塊，文字會繞著float物件，但區塊本身會被壓在float物件下方，可使用clear清除。
#### clear
清除元素對浮動的影響。

#### 浮動問題
1. 當前方元素為浮動時，後方元素會受到影響
> 解法
> 設定clear

2. 當子元素都是浮動時，父元素高度會歸零（父元素崩蹋）
> * 解法一：
> 設定高度
> * 解法二：
> 設定overflow:auto到父元素
> * 解法三：
> 設定clearfix到父元素
> * 解法四：
> 設定display: flow-root到父元素

##### clearfix
```css
.clearfix::after {
    content: "";
    display: block;/*可使用table*/
    clear: both
}
```

#### 虛擬元素 before , after
在元素內的前方、後方產生一個虛擬的元素，產生的為行內元素，一定要加上content屬性。
```css
h1::before {
    content:"before";
}
h1::after {
    content:"after";
}
```

### 置中
#### line-height置中
#### table置中
#### inline-block置中
#### padding置中

### 選取器
#### 後代選取器
#### 子代選取器
# 響應式網頁 0611 課程綱要
## CSS排版
### Flex 彈性盒子

#### display
```css
.container {
    display: flex;
}
```

#### flex-flow
- flex-wrap 換行 
- flex-direction 排列方向

```css
.container {
    display: flex;
    flex-wrap: wrap;
    /*
        no-wrap 不換行
        wrap    換行
        
    */
    flex-direction: row;
    /*
        row            橫排
        row-reverse    橫排反轉
        column         直排
        column-reverse 直排反轉
    */
}
```


#### justify-content
```css
.container {
    display: flex;
    justify-content: center;
    /*
        flex-start     置左
        center         置中
        flex-end       置右
        space-around   分散對齊，每個區塊左右具有間距
        space-between  分散對齊，左右兩側區塊貼壁
        space-evenly   分散對齊，均分每個間距
    */
}
```
> space-evenly是後期加入的值，相容性差不建議使用

#### align-items 
```css
.container {
    display: flex;
    align-items: center;
    /*
        flex-start    置頂
        center        置中
        flex-end      置底
        stretch       拉伸
        baseline      文字基準線
    */
}
```
#### flex
- flex-grow 元件伸展性
- flex-shrink 元件壓縮性
- flex-basis 元件基準值
```css
.box {
    flex: 0 0 calc(100% / 3);
    /* flex: flex-grow flex-shrink flex-basis */
}
```
#### order
設定flex內物件的排序，數字越小越前面
```css
.box:nth-of-type(1){
    order: 2;
}
.box:nth-of-type(2){
    order: 1;
}
```

### 選取器
#### nth-of-type()

### 定位Position
- 靜態定位 Static：預設值
    
- 相對定位 Relative：以自己為基準做偏移、順序的切換
    
- 絕對定位 Absolute：以視窗為基準做偏移、順序的切換，但會被相對定位所影響。滾動時會跟著卷軸移動
- 固定定位 Fixed：以視窗為基準做偏移、順序的切換，不會被相對定位所影響。滾動時會固定在視窗上
- *黏性定位 Sticky
#### 可用屬性
- top
- bottom
- left
- right
- z-index
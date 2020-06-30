# CSS效果
## transition 過場效果

- transition-property           屬性
- transition-duration           動畫秒數
- transition-delay              延遲
- transition-timing-function    速度變化
    - ease
    - ease-in
    - ease-out
    - ease-in-out
    - linear
- transition
```css
.box {
    transition-property: width;
    transition-duration: .3s;
    transition-delay: 1s;
    transition-timing-function: ease-in-out;
}
/* 等同於 */
.box {
    transition: width .3s 1s ease-in-out;
}
```

## transform 變形
- scale()       比例
- rotate()      旋轉
- translate()   位移
- skew()        傾斜

```css
.box {
    transform: scale(.5,.5);
    transform: rotate(45deg);
    transform: translate(100px,300px);
    transform: skew(30deg,45deg);

    transform: scale(.5)rotate(45deg)translate(100px,100px)skew(15deg,0);
}
```
> 使用rotate時，xyz軸也會跟著旋轉
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
# margin塌陷和合并
## 总结一下：
### 一、外边距塌陷
两个嵌套关系的（父子关系）块元素，当父元素有上外边距或者没有上外边距（margin-top），子元素也有上外边距的时候。两个上外边距会合成一个上外边距，以值相对较大的上外边距值为准。
```
index.html
<div id="father">
        <div id="son"></div>
</div>
CSS
#father{
    height: 100px;
    width: 100px;
    background-color: brown;
}
#son{
    width: 50px;
    height: 50px;
    margin-top: 20px;
    background-color: chartreuse;
}
```
解决方案：<br/>
1. 给父元素设置外边框（border）或者内边距（padding）(不建议)
```
{
    设置border，单纯用border-width还不行，需要设置线的类型;
    父元素设置border和padding，会把盒子撑大。
}
```
2. 触发BFC(推荐)
### 二、内边距塌陷
给一个元素设置下外边距（margin-bottom），并同时给一个元素设置上外边距（margin-top）。两个元素之间的距离不等于这两个外边距之和，而是等于其中最大的一个外边距。<br/>
解决方案：
1. 只设置其中一个元素的margin值即可（推荐）项目中一般都会设置
2. 设置父盒子，触发BFC(不加父盒子不行)
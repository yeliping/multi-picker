## DateSelectorPro - 日期选择器优质版

#### 优质的主要表现在:
> 优化版的自定义功能不仅是【单位】自定义

> 【时间范围】也可以自定义,自定义的时间可以精确到分钟，并尽可能的进行数据合法性校正

> 例如可以设置【2011年13月(-27)日 102时12分 ~ 2020年10月21日 20时20分】的效果

<br/>
### 0.[在移动端下打开demo](https://appianz.github.io/multi-picker/DateSelectorPro.html)
### 1.如何引用

> sass文件:引用DateSelectorPro/DateSelectorPro.scss

> css文件:引用DateSelectorPro/DateSelectorPro.css

> js文件:引用DateSelectorPro/DateSelectorPro.js

### 2.如何使用

**html的基本格式：**
```html
<link rel="stylesheet" type="text/css" href="./DateSelectorPro.css"/>
<body>
    <input id="date-selector-input" type="text" readonly/>
    <div id="targetContainer"></div>
</body>
```

**调用js的基本格式：**
```html
<script src="./DateSelectorPro.js"></script>
<script>
    new DateSelector({ ... });
</script>
```

**参数配置：**

| 参数 | 字符类型  |  取值  | 说明 | 
| -----| -----| -----| -----|
|  **input**    |  {String} | *eg:'date-selector-input'* | 点击触发插件的input框的id |
|  **container**    |  {String} |*eg:'targetContainers'*| 插件即将插入的容器id |
|  **type**    | {Number} |0 或 1 | 0为自定义插件的日期单位(不带tab切换)，1为固定插件的日期单位为【年月日】【时分】(带tab切换) |
|  **param**  |  {Array} |*eg:[1,1,0,0,0]*| 设置单位，元素分别对应设置['year','month','day','hour','minute'],1为需要，0为不需要,需要为连续的1 |
|  **beginTime**   |  {Array} |*eg:[2011,3,27,12,12]      2011年3月27日12点12分*| 设置开始时间点,空数组默认设置成1970年1月1日0时0分开始，数组的值对应param参数的对应值。 |
|  **endTime** |  {Array} |同beginTime| 设置结束时间点,空数组默认设置成次年12月31日23时59分结束，数组的值对应param参数的对应值。 |
|  **recentTime**  |  {Array} |同beginTime| 设置当前时间点,空数组默认设置为系统当前时间，数组的值对应param参数的对应值。 |
|  **callbackfuc**   |  {function} |*function(arr){alert(arr)}*| function(arr){} 回调函数，可以自定义结果格式化|

* type = 0 自定义单位，【年月日时分】的自定义任意组合

 ![img2.](http://7xqsim.com1.z0.glb.clouddn.com/DateSelector5.jpeg) 

* type = 1 带tab切换，固定单位【年月日时分】的固定样式

 ![img1.](http://7xqsim.com1.z0.glb.clouddn.com/DateSelector4.jpeg) 

### 3.有什么优越性？

带有加速度的滑动 (•‿•)

能够动态设置任意开始和结束【时!间!点!】 (•‿•)

> 是的,你可以设置任何尴尬的时间了~ 比如:【2016-11-11 11:11 ~ 2016-12-12 12:12】

能够任意设置时间单位的组合 (•‿•) 

> "年月日"  OR  "月日时分"  OR  "年月日时分"

能够切换固定样式和自定义样式,简化参数 (•‿•)

能利用我的模型处理更多、更自由的联动 (•‿•)

> 比如城市多级联动，请移步[自定义json选择器 - MultiPicker.](https://github.com/AppianZ/multi-picker/tree/master/MultiPicker)

#### Trust Me. 

### 4.有什么局限性？

> 样式主题可能和你的产品风格不符，可以通过更改sass中的全局变量来解决问题 >.<

> 如果你只需要设置年份范围，不需要精确到后面的时间单位，请移步[日期选择器简易版 DateSelectorSimple.js](https://github.com/AppianZ/multi-picker/tree/master/DateSelectorSimple)

> 如果遇到什么神bug,不要着急。这时候,请对我发起issue~ 一定让您满意！

>  我是嘉宝Appian，一个卖萌出家的算法妹纸。

#### Trust Me. Again.


# 获取手机拍摄照片的经纬度及详细位置的python脚本

## 说明

本脚本的源码是xingag大佬的，本人只是稍作了改动，及添加了一些说明方式，使得脚本能够应用于更多场合。

[xingag大佬的github](https://github.com/xingag/)
[本人的github](https://github.com/FDlucifer/)


### 脚本使用说明

* 1.先从高德开放平台上注册后再申请一个key，如下图所示。

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location.jpg)

* 2.如下几图所示修改main.py的源代码,使其对应正确的key和要分析的图片地址。

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location2.jpg)

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location3.jpg)

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location4.jpg)

* 3.运行代码前，先执行下面的代码安装exifread库。

``` bash
pip3 install exifread
```
该库是识别图片元数据的库，使用 exifread 库可以直接读取图片文件，获取到图片的元数据，包含经度、纬度、南北纬方向、东西经方向和拍摄时间。

* 4.运行代码时，main.py和position_utils.py必须放在同一目录下。

因为通过 GPS 获取的经度、纬度和高德地图的坐标存在一定的误差，这里需要用position_utils.py脚本把坐标转换为「火星坐标系」。

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location5.jpg)

## 最后附上一张效果图

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/location6.jpg)

###**<font color="red">牛批哄哄的有没有?</font>**

#### 最后觉得不错，请按下图扫码捐助，谢谢。

![](https://raw.githubusercontent.com/wiki/FDlucifer/FDlucifer.github.io/wechat-qcode.jpg)
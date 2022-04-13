# 叮咚小程序自动预约
本程序为自动预约叮咚买菜小程序是的商品，无需配置代码环境，开箱即用

## 使用教程
1. 在release下载已经打包好的程序并打开, [下载](https://gitee.com/wenxiansen/ddmc-gui/tags)
1. 选用Charles抓包填入参数
2. 执行即可

## 注意事项

1. 如果在6点和8点30（进APP看公告有写开放时间）没买到不要一直跑程序，长时间并发接口会被对方拉黑到IP黑名单中，接口返回405,一般一分钟内没预约到就建议关闭程序

## 快捷抓包

忘记小程序已经有PC版了，手机进入小程序右上角3个点->在电脑中打开即可，送上一个参考文章https://blog.csdn.net/z2181745/article/details/123002569 比手机抓包方便太多。

注意事项
1. Charles安装和配置好后再打开或重新打开电脑端叮咚小程序，如果在之前打开可能会抓不到
2. 如果使用电脑端小程序抓包，则不要去碰手机微信里的叮咚小程序，否则session会失效，反过来也一样，其他操作在app上操作不影响，但不能同时在两个端的小程序操作，互斥

## 版本
2022041302版本更新日志
1. 修复只有一个地址时的报错
2. 优化线程打印
exe中session、referer、device_id将从header中读取
![图片](./header.png)
exe中devices将从header中读取
![图片](./params.png)
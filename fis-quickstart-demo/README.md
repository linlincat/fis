本实例来源于百度官网，学习来源fis.baidu.com

fis-quickstart-demo
===================

fis-quickstart-demo是FIS的快速上手示例，请配合[文档](http://fis.baidu.com/docs/beginning/getting-started.html)使用

资料压缩

如果觉得参数输入比较麻烦，实际也支持参数压缩，更多的参数:fis release -h
fis release --optimize  (fis release -o)

添加文件版本
fis release --md5 (fis release -m)  压缩切添加版本(fis release --optimize --md5)或者(fis release -om)

资源合并
设置打包[测试的时候，不知为何没安装插件是，无法进行打包合并。即使效果没报错，也不生成pkg这个文件目录]
fis release --optimize --md5 --pack (fis release -omp)
//通过资源合并，已经可以对成功将脚本资源和样式表资源进行了合并

合并图片
用于图片合并的插件csssprites已经在FIS中内置了，因此无需安装，只需要在fis-conf.js的配置中开启即可.

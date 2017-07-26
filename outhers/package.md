1 打开Installshield2015

2 打开项目文件

路径位于（[\\\\192.168.0.250\\ShareDir\\工具\\打包工程\\TestESDesktop下的TestESDesktop.ism](../../../../打包工程/TestESDesktop下的TestESDesktop.ism)）

打开项目

![](outhers/media/3e93a6a30e1003e1968bb75586952abe.png)

3 修改参数

大多数参数已经设置好了，这里仅需设置待打包程序的目录，如（\\\\192.168.0.250\\ShareDir\\xzp\\Debug20170711\\Debug20170711）注意此目录下必须直接包含程序相关的内容。

![](outhers/media/66556375ce713af5b228e2beb43bcba8.png)

在Debug目录发生很大变化时（如底层新增了接口，这个需要应用层或者底层开发确定），需要重新添加Debug目录而不是仅仅修改路径。如下图，重新添加Debug。

![](outhers/media/f9e48d8b57ef68bddc30a285cd1113a6.png)

4 运行打包工程

![](outhers/media/e7fc2e52f10cc1b8c09d0f67d40e818f.png)

或者点击build installation

![](outhers/media/6eb6d8baae3c0a01644b13c8e0e46d4e.png)

5 获取最终的打包结果

打包的结果位于项目文件下，如D:\\InstallShield 2015
Projects\\TestESDesktop\\PROJECT_ASSISTANT\\SINGLE_EXE_IMAGE\\DiskImages\\DISK1，拷贝出来发布即可

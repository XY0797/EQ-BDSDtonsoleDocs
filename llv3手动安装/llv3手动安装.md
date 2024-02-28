# llv3手动安装

## 1. 下载文件

安装llv3本体所需要的文件：

[LeviLamina](https://github.com/LiteLDev/LeviLamina)

[PreLoader](https://github.com/LiteLDev/PreLoader)

[PeEditor](https://github.com/LiteLDev/PeEditor)

llv3加载旧版本插件需要的文件：

[LegacyScriptEngine](https://github.com/LiteLDev/LegacyScriptEngine)

[LegacyMoney](https://github.com/LiteLDev/LegacyMoney)

[LegacyRemoteCall](https://github.com/LiteLDev/LegacyRemoteCall)

[LegacyParticleAPI](https://github.com/LiteLDev/LegacyParticleAPI)

到release里面下载最新的发行版本

![图片](image.png)

![图片](image-1.png)

![图片](image-2.png)

其它的大同小异

也可以到action里面下载最新的开发版

但是有时候会遇到文档更新：

![图片](image-3.png)

![图片](image-4.png)

碰到上图这种说明是文档更新，这时候需要换一个action：

![图片](image-5.png)

![图片](image-6.png)

LegacyScriptEngine比较特殊，两个都要下载，其它的就是只下载一个就行

## 2. 安装

### 2.1 llv3本体

llv3需要9个文件：

![图片](cab2b9a6e21424c770e5c719bcc2e37f.png)

先全部解压：

![图片](36b6e1d6e13b8d5a15c551df190f15a1.png)

这三个拖入BDS文件夹：

![图片](39dc9b0bfa1c96d6e5bea12924c3bdb9.png)

![图片](31228866ee4b71287fd49768663d2c12.png)

![图片](f5b9b4b55a7ef6463dc2b0215ba07a06.png)

然后像llv2一样运行这个：

![图片](e1963d1285eb94f2b7e41f5209bef7a4.png)

跑一遍，然后stop关服：

![图片](8c5f891b5585c3a059a24fed17971763.png)

这样子LLv3的本体就搞好了，但是不能加载插件

### 2.2 旧插件加载器

这5个文件：

![图片](50aba6a29b6b3a2ab5dcf0f11a6de756.png)

![图片](3cf7bcb78d9744ae6b854a493ae5f0bd.png)

![图片](88db929133da9af21e567c65c0b4c3af.png)

![图片](16de590d5e0ed4a9758d4ffdf3956e13.png)

![图片](720e0cfcb9bf2bdf42834c33c0919e08.png)

放到这里：

![图片](7b3c28a24ed41999eabd1316142069cb.png)

运行一次，然后stop：

![图片](40a6da3da3627e434f29801d81b1258b.png)

这样子插件加载器就搞定了

### 2.3 插件安装

然后把你的js/lua插件(注意！DLL插件请放弃)，一次一个的放入plugins文件夹

我这里已经确认了这几个插件能在llv3上跑，所以说同时放了两个

![图片](4dda868e0a83a3c0e5fa7622f5f14133.png)

放入后必须运行一次，并且这一次必须加载完成就stop：

![图片](17331d4e933ce681e79fc7e5a241e5cd.png)

然后再运行一次，这一次插件就能加载了

![图片](069d0bec16cf3bc4dd53e326b54b2bc1.png)

然后进服务器检查功能是否正常，后台是否报错

报错或功能不正常就说明插件没用了，如果你不会开发的话就只能放弃

重复上面过程，完成插件迁徙

### 2.4 数据迁移

BDS常规的数据：

![图片](e75890937718927f15a5a9fa10dd2091.png)

ll经济插件的数据：

![图片](95b17acf4bd355284918faedcdba1cad.png)

至于插件的数据我还没有研究过，所以只能你们自己探索了
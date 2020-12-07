<!--
 * @Description: 
 * @Author: HCQ
 * @Company(School): UCAS
 * @Date: 2020-10-04 18:17:00
 * @LastEditors: Please set LastEditors
 * @LastEditTime: 2020-12-07 10:27:12
-->
# pcl
PCL（Point Cloud Library）点云库  **个人开发环境：Ubuntu18.04**

**墙裂建议先看下：[PCL(Point Cloud Library)学习指南&资料推荐](https://www.yuque.com/huangzhongqing/pcl/rdk5k8)**

@[双愚](https://github.com/HuangCongQing/pcl-learning) , 若fork或star请注明来源

>* 点云数据的处理可以采用获得广泛应用的Point Cloud Library (点云库，PCL库)。
>*  PCL库是一个最初发布于2013年的开源C++库。它实现了大量点云相关的通用算法和高效的数据管理。
>* 支持多种操作系统平台，可在Windows、Linux、Android、Mac OS X、部分嵌入式实时系统上运行。如果说OpenCV是2D信息获取与处理的技术结晶，那么PCL在3D信息获取与处理上，就与OpenCV具有同等地位
>*  PCL是BSD授权方式，可以免费进行商业和学术应用。

* 英文官网：https://pcl.readthedocs.io/projects/tutorials/en/latest/#
    * https://pointclouds.org/
* GitHub：https://github.com/PointCloudLibrary/pcl
    * 学习基于pcl1.9.1：https://github.com/PointCloudLibrary/pcl/tree/pcl-1.9.1



* **个人笔记：https://www.yuque.com/huangzhongqing/muam1n**

Tips:
* ubuntu下使用PCL，需要写CMakeLists.txt文件，然后编译才可以生成可执行文件.
* 可执行文件在build文件夹下，所以运行可执行文件时，后面添加参数的pcd文件，应放在build文件夹下才能获取到。（注意文件路径）



## 目录contents
a graph of code libraries
* [00base](00base)
##### step1
* [01common](01common )

##### step2
* [02kdtree k维tree](02kdtree)
* [03octree 八叉树](03octree)
* [04search](04search)

* [05sample consensus  抽样一致性模块](05sampleconsensus抽样一致性模块)
* [06range-images深度图像](06range-images深度图像)
* [07 ...]()
##### step3
* [08 io 输入输出](08IO输入输出)
* [09 filters 滤波](09filters滤波)
* [10 features 特征](10features特征)


##### step4
* [11 surface表面 ](11surface表面 )
* [12 segmentation分割](12segmentation分割)
* [13 recognition识别](13recognition识别)
* [14 registration配准](14registration配准)
* [15 visualization可视化](15visualization可视化)
* [16 keypoints关键点](16keypoints关键点)
* [17tracking](17tracking )

## 编译过程
```shell
mkdir build
cd build
cmake .. // 对上一级进行编译
make  // 生成可执行文件命令
./executedemo  // 运行可执行文件
```


## 相关链接
* 公众号：点云PCL
* https://github.com/Yochengliu/awesome-point-cloud-analysis
* https://github.com/QingyongHu/SoTA-Point-Cloud
* https://github.com/PointCloudLibrary/pcl
* 参考书籍：点云库PCL学习教程，朱德海，北京航空航天大学出版社

**入门资料：**

- **视频**：[bilibili-PCL点云库官网教程](https://space.bilibili.com/504859351/channel/detail?cid=130387)
- **点云库PCL学习教程书籍每章总结：**[https://github.com/MNewBie/PCL-Notes](https://github.com/MNewBie/PCL-Notes)
- 百度网盘资料：

链接：[https://pan.baidu.com/s/1ziq8s_kj5QpM8eXO_d6RJg](https://pan.baidu.com/s/1ziq8s_kj5QpM8eXO_d6RJg)<br />提取码：g6ny<br />

**代码实践资料：**

- 官方各模块示例(和对应的对象函数对照着看)【英文】：[https://pcl.readthedocs.io/projects/tutorials/en/latest/#](https://pcl.readthedocs.io/projects/tutorials/en/latest/#)
- 官方各模块对应的对象和函数【英文】：
   - [https://pointclouds.org/documentation/modules.html](https://pointclouds.org/documentation/modules.html)
   - [https://pointclouds.org/](https://pointclouds.org/) 点击网站中的12宫图，没一格对应一个模块的对象函数详解
- [黑马机器人系列文档：PCL-3D点云](http://robot.czxy.com/docs/pcl/)：[http://robot.czxy.com/docs/pcl/](http://robot.czxy.com/docs/pcl/)
- [CSDN博主系列文章PCL学习(64篇)](https://www.cnblogs.com/li-yao7758258/category/954066.html)：[https://www.cnblogs.com/li-yao7758258/category/954066.html](https://www.cnblogs.com/li-yao7758258/category/954066.html)

### License

Copyright (c) [双愚](https://github.com/HuangCongQing/pcl-learning). All rights reserved.

Licensed under the [MIT](./LICENSE) License.

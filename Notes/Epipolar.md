# 对极几何｜Epipolar Geometry

对立体视觉建模的一种方法(约束)，使得立体匹配问题有一个最优解

![image.png](https://upload-images.jianshu.io/upload_images/12014150-3b9134809f9124d6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

`X`: 三维空间点(研究对象)
`C、C’`: 两摄像机中心
`x、x’`: `X`在两摄像机成像平面的投影点

- **基线**：两摄像机光心的连线 `CC’`
- **对极点**：一幅视图中另一个摄像机中心的像(基线与两成像平面的交点) `e、e’`
- **对极平面**：包含基线的平面(以基线为轴转动) `CXC’`
- **对极线**：对极平面与成像平面的交点 `xe、x'e'`

## 极线约束

如果世界点X在图像1上的像点x已知，那么世界点X在图像2上的像点必然在极线`x'e'`上

**缩小特征点匹配时搜索范围**：将对应点匹配从整幅图像寻找压缩到在一条直线上寻找对应点（点对线的约束）
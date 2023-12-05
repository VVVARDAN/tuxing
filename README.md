# Seam Carving 
## 媒体计算小作业2
通过像素值给定一幅4x4的灰度图像$I$

```
0 0 1 0
0 1 2 1
1 2 2 2
2 2 2 2
```

按照课上讲述的Seam Carving论文（Seam Carving for Content-Aware Image Resizing）中，图像重要性用$|\frac{\partial I}{\partial x}|+|\frac{\partial I}{\partial y}|$表示，具体实现过程中，使用一阶差分近似：
当$0\le i< 3$时:
$$ \frac{\partial I(i,j)}{\partial x} = I(i+1,j)-I(i,j)$$

当$i=3$时:
$$ \frac{\partial I(i,j)}{\partial x} = I(i,j)-I(i-1,j)$$

当$0\le j< 3$时:
$$ \frac{\partial I(i,j)}{\partial y} = I(i,j+1)-I(i,j)$$

当$j=3$时:
$$ \frac{\partial I(i,j)}{\partial y} = I(i,j)-I(i,j-1)$$

问：对于上述图像，先纵向删除一个细缝。请给出纵向删除一个细缝后的图像结果。注：大小变为4x3（4行3列）

```

```

再横向删除一个细缝（变为3x3）后的图像结果是什么？

``` 

```
请给出结果和解答过程。若有多种可能细缝，任选一种删除即可。



# 数据结构与算法笔记

## 导语

### 如何一组数据排序 ？

快速排序？

> 同样是 O(nlogn)复杂度的排序算法当中，快速排序是最快的， 应该是'正确'的

但是它不是最优的， 解决算法问题的时候，更多的是要考虑场景/环境

> 这组数据有没有什么具体特征,比如说数据包含大量的重复要素？

这种情况下三路快排的是更好的选择

> 当然如果能肯定这组数据大多是独特的

快速排序理应是最好的

> 是否大部分的数据距离正确的位置都很近，也就是说近乎是有序的？

这种情况下插入排序是最好的选择

> 是否这组数据的取值非常有限？

这种情况下计数排序是更好的选择

> 对排序有什么额外的要求, 例如是否需要稳定排序？

如果是的话，快排并不是很好的选择，而归并排序的很好的选择

> 另外，数据的存储结构是怎么样的？

快排非常依赖数组的随机存储的特征， 如果是使用链表存储，此时归并
排序的是好的选择

> 数据的大小呢？ 足以装载在内存中吗？

此时就需要考虑外排序的方法

### 选择合适的 OJ(Online Judge)

> Leetcode

> HackerRank

这两个比较适合面试算法刷题

> CodeForces

> Topcoder

> CodeChef

这三个比较偏竞赛类

**不要忽略暴力解法 往往是优化方式的起点**

### 优化算法

优化思路

- 常见的算法思路
- 常见的数据结构
- 空间和事件的交换(哈希表)
- 预处理信息(排序)
- 在瓶颈处寻找答案

实际编写

- 极端条件判断
- 代码规范，模块化，复用性

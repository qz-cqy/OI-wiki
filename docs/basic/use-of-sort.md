本页面将简要介绍排序的用法。

## 降低时间复杂度

使用排序预处理可以降低求解问题所需要的时间复杂度。

???+note "示例：检查给定数列中是否有相等的元素"
    考虑一个数列，你需要检查其中是否有元素相等。
    
    一个朴素的做法是检查每一个数对，并判断这一对数是否相等。时间复杂度是 $O(n^2)$ 。
    
    我们不妨先对这一列数排序，之后不难发现：如果有相等的两个数，它们一定在新数列中处于相邻的位置上。这时，只需要 $O(n)$ 地扫一遍新数列了。
    
    总的时间复杂度是排序的复杂度 $O(n\log n)$ 。

## 作为查找的预处理

排序是 [二分查找](./binary.md) 所要做的预处理工作。在排序后使用二分查找，可以以 $O(\log n)$ 的时间在序列中查找指定的元素。

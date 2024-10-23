## 思维导航

* [前言](https://github.com)
* [实现原理](https://github.com)
* [代码实现](https://github.com)
* [最后总结](https://github.com)
* [C\#算法实战入门指南](https://github.com)

:[飞数机场](https://ze16.com)## 前言


线性查找算法是一种简单的查找算法，用于在一个数组或列表中查找一个特定的元素。它从数组的第一个元素开始，逐个检查每个元素，直到找到所需的元素或搜索完整个数组。线性查找的时间复杂度为O(n)，其中n是数组中的元素数量。


## 实现原理


1. 从列表的第一个元素开始，逐个检查每个元素。
2. 如果当前元素等于目标元素，则返回该元素的索引。
3. 如果遍历完整个数组都没有找到匹配的值，则返回一个表示未找到的值（通常是\-1）。


## 代码实现



```
        public static void LinearSearchRun()
        {
            int[] arr = { 2, 3, 4, 10, 40, 50, 100, 77, 88, 99 };
            int target = 100;

            int result = LinearSearch(arr, target);

            // 输出结果
            if (result == -1)
            {
                Console.WriteLine("元素未找到");
            }
            else
            {
                Console.WriteLine($"元素在索引 {result} 处找到，index = {result}");
            }
        }

        /// 
        /// 线性查找函数
        /// 
        /// arr
        /// target
        /// 
        public static int LinearSearch(int[] arr, int target)
        {
            // 遍历数组
            for (int i = 0; i < arr.Length; i++)
            {
                // 如果找到目标值，返回其索引
                if (arr[i] == target)
                {
                    return i;
                }
            }
            // 如果没有找到，则返回-1
            return -1;
        }

```

## 最后总结


线性查找算法简单易懂，适用于小规模数据集或无序数据集。其主要优点是实现简单，不需要对数据进行排序。然而，由于其时间复杂度为O(n)，对于大规模数据集，效率较低。对于大规模数据集或需要频繁查找的场景，可以考虑使用更高效的查找算法，如二分查找（适用于有序数据集）或哈希查找。


## C\#算法实战入门指南


[https://mp.weixin.qq.com/s/XPRmwWmoZa4zq29Kx\-u4HA](https://github.com)



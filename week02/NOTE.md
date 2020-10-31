# 哈希表 Hash table
* 碰撞
    * 不同值,hash后相同
    * 解决方案，节点变链表
    * size越小，越容易碰撞，时间复杂度越高

* insert/search/delete O(1)

# 树
* 二叉树
    * 前序遍历(Pre-order)：根-左-右
    * 中序遍历(In-order)：左-根-右
    * 后序遍历(Post-order)：左-右-根
* 二叉搜索树
    * insert/search/delete O(log n)
    
# 堆 Heap
* 迅速找到 MIN或MAX
* 二叉堆 (完全二叉树)
* fib堆
* 大顶堆
    * find-max O(1)
    * delete-max O(logN)
    * insert/create O(logN) / O(1)
* 放到数组里
    * 索引为i的左子的索引是：2*i+1
    * 索引为i的右子的索引是：2*i+2
    * 索引为i的父的索引是：floor((i-1)/2)
* insert
    * 放到最尾部
    * 逐步向上做替换,if > 父, 和父替换 (heapifyUp)
    * 最大操作数为树的深度，即O(logN)
* delete-max
    * 移除顶部元素
    * 将尾部元素i放到顶部
    * 逐步将i与左右子中大者替换 (heapifyDown)
    * 最大操作数为树的深度，即O(logN)
* 工程中-优先级队列(priority_queue)

# 图 Graph(V, E)
* V - vertex: 点
* E - edge: 边
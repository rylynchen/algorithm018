# 数据结构
* 一维
	* 数组 array
        * prepend/append/search O(1)
        * insert/delete O(n)
	* 链表 linked list
        * prepend/append/insert/delete O(1)
        * search O(n)
	* 栈 stack
        * 先进后出
        * insert/delete O(1)
        * search O(n)
	* 队列 queue
        * 先进先出
        * insert/delete O(1)
        * search O(n)
	* 双端队列 deque (Double-End Queue)
        * insert/delete O(1)
        * search O(n)
	* 集合 set
	    * insert/delete/lookup O(1)
	* 字典 map
	    * insert/delete/lookup O(1)
	    * 碰撞
            * 不同值, hash后相同
            * 解决方案，节点变链表
            * size越小，越容易碰撞，时间复杂度越高
* 二维
	* 树 tree
	    * 时间
	        * insert/delete/search O(log n)
	    * 遍历
            * 前序遍历(Pre-order)：根-左-右
                * 第一个节点是root
            * 中序遍历(In-order)：左-根-右
                * root左边是左子树,root右边是右子树
                * 已知前序遍历和中序遍历，可推断出整个树
            * 后序遍历(Post-order)：左-右-根
	* 图 graph(V, E)
        * V - vertex: 点
        * E - edge: 边
	* 二叉搜索树 binary search tree
	    * insert/delete/lookup O(log n)
	* 堆 heap
        * 迅速找到 MIN(小顶堆)或MAX(大顶堆)
        * 二叉堆 (完全二叉树)
        * fib堆
        * 大顶堆
            * find-max O(1)
            * delete-max O(log n)
            * insert/create O(log n) / O(1)
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
	* 并查集 disjoint set
	* 字典树 trie
* 特殊
	* 位运算 Bitwise
	* 布隆过滤器 BloomFilter
	* LRU cache
	
# 算法
* branch : if-else, switch
* iteration : for, while, loop
* 递归 recursion
* 搜索 search : 深度优先 Depth first search, 广度优先 Breadth first search
* 动态规划 Dynamic Programming
* 二分查找 Binary search
* 贪心 Greedy
* 数学 Math, 几何 Geometry
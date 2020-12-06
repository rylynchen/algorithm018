# 字典树 Trie
# 并查集
```
def init(p):
    for i in range(n)
        p[i] = i

def union(self, p, i, j):
    p1 = self.parent(p,i)
    p2 = self.parent(p,j)
    p[p1] = p2

def parent(self, p, i):
    root = i
    while p[root] != root:
        root = p[root]
    while p[i] != i
        x=i; i=p[i]; p[x]=root
    return root
```

# A* search
```
def AstarSearch(graph, start, end):
    pq = collections.priority_queue()
    pq.append([start])
    visited.add(start)

    while pq:
        node = pq.pop()
        visited.add(node)

        process(node)
        nodes = generate_related_nodes(node)
        unvisited = [node for node in nodes if node not in visited]
        pq.push(unvisited)
```

# AVL
* 平衡二叉搜索树
* 每个节点需要存balance factor = {-1,0,1}
* 平衡因子： 左子树高度 - 右子树高度
* 旋转操作
    * 左旋
    * 右旋
    * 左右旋
    * 右左旋

# 红黑树
* 近似平衡的二叉搜索树,任意节点左右子树高度差小于两倍
* 每个节点是红或黑
* 根节点是黑
* 每个叶子节点是黑
* 不能有相邻居接的两个红色节点
* 从任意节点到其每个叶子的所有路径都包含相同数据的黑节点
* 读多用AVL,写多用红黑树
* AVL应用: database
* 红黑树应用: map, set
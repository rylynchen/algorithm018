# 搜索-遍历
* 每个节点都要访问一次
* 每个节点仅访问一次
* 顺序不同
    * 深度优先：dfs (depth first search)
    * 广度优先: bfs (breadth first search)
    * 优先级优先
   
* DFS模版
    * 二叉
    ```
    def dfs(node):
        if node in visited:
            return
        visited.add(node)
        # logic code here
        dfs(node.left)
        dfs(node.right)
    ```
    * 多叉
    ```
    # 递归
    def dfs(node, visited):
        if node in visited:
            return
        visited.add(node)
        # logic code here
        for next_node in node.children():
            if not next_node in visited:
                dfs(next_node, visited)
    # 非递归
    dfs (self, tree):
        if tree.root is None:
            return
        visited, stack = [], [tree.root]
        while stack:
            node = stack.pop()
            visited.add(node)
            # logic code here
            stack.push(node.children)
    ```
* BFS模版
    ```
    def bfs(graph, start, end):
        queue = []
        queue.append([start])
        visited.add(start)
        while queue:
            node = queue.popleft()
            visited.add(node)
            # logic code here
            queue.push(node.children)
    ```
# Task01-图机器学习导论

**图**，用于描述数据间的**关联**。
在图机器学习中，图包括：节点（Node）和边（Edge）。

### 特点
一般的机器学习和深度学习，假定样本间是**独立同分布**的，**图机器学习**则不然，它可以捕捉样本间的**关联**。

### 难点
这是优势，但同时也带来了难点：
- 输入尺寸任意、拓扑复杂
- 没有固定的节点顺序和参考锚点
- 动态变化
- 具有多模态特征（比如在歌曲推荐中，一首歌包括可能包括音频、歌曲年代、歌手信息、MV等各维度features）

### 要点
**映射**是所有机器学习、深度学习算法的要点，图机器学习也不例外。它通过**表示学习(Representation Learning)/图嵌入(Node Embedding)**，把复杂数据(node)**映射**成一个包含**节点语义信息/连接关系**的**嵌入向量**。
<summary>Representation Learning</summary>
    <img src="fig/CS224W&Representation Learning.png" alt="Representation Learning" width="256" height="256">

这种图嵌入的映射，可以自动学习特征（类似CNN），无需人工特征工程。(end-to-end)

### 工具库
- PyG（PyTorch Geometric）：官方库，和PyTorch类似
- GraphGym
- NetworkX
- DGL：李沐推荐，适合进行学术研究
- 图数据可视化：AntV、Echarts、GraphXR

### 应用
根据不同层次（Node, Edge, Subgraph, Graph-level）的任务，有不同的应用，举例如下：
<summary>Different tasks</summary>
    <img src="fig/Different tasks.png" alt="Different tasks" width="256" height="256">


### 图的商业价值
- 图是最优质的长期资产
- 网络效应是一个企业最深的护城河

### 图数据挖掘项目
- ReadPaper：专业的学术讨论社区，实现文献引用网络
- CONNECTED PAPERS：可以展示文献引用网络
- BIOS：生物医学知识图谱
- Hypercrx：展示项目关系网络图、项目活跃开发者协作网络图
- OpenRank：一种基于异质网络的价值评价算法
- 开源项目和开源企业排行榜：https://open-leaderboard.x-lab.info

<p style="text-align: right; font-size: 15px;"><a href=20230213第46期CS224W图机器学习.md>[Homepage] ----- </a><a href=20230213第46期CS224W图机器学习.md>[Previous: Homepage] ----- </a><a href=Task02-图的基本表示和特征工程.md>[Next: Task02]</a></p>
# BFM 维基百科翻译

## Bellman–Ford算法 <a id="firstHeading"></a>

维基百科，自由的百科全书[跳转到导航](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#mw-head)[跳转到搜索](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#p-search)

| Bellman–Ford算法 |  |
| :--- | :--- |
| 类 | [单源最短路径问题](https://en.wikipedia.org/wiki/Single-source_shortest_path_problem)（针对加权有向图） |
| 数据结构 | [图形](https://en.wikipedia.org/wiki/Graph_%28data_structure%29) |
| [最坏情况下的表现](https://en.wikipedia.org/wiki/Best,_worst_and_average_case) | { displaystyle  Theta（\| V \|\| E \|）}![{ displaystyle  Theta&#xFF08;\| V \|\| E \|&#xFF09;}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0465422c67bedf2d1659571f5797b3c9c54ed9ad) |
| [最佳情况下的表现](https://en.wikipedia.org/wiki/Best,_worst_and_average_case) | { displaystyle  Theta（\| E \|）}![{ displaystyle  Theta&#xFF08;\| E \|&#xFF09;}](https://wikimedia.org/api/rest_v1/media/math/render/svg/fee8b4657c1eb491bc9d05378522ddc12ddac5fc) |
| [最坏情况下的空间复杂度](https://en.wikipedia.org/wiki/Best,_worst_and_average_case) | { displaystyle  Theta（\| V \|）}![{ displaystyle  Theta&#xFF08;\| V \|&#xFF09;}](https://wikimedia.org/api/rest_v1/media/math/render/svg/d6859084635373622fc54329d559928d0d564d42) |

| [图](https://en.wikipedia.org/wiki/Graph_traversal)和 [树 搜索算法](https://en.wikipedia.org/wiki/Tree_traversal) |
| :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">
        <ul>
          <li><a href="https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning">a &#x2013; b</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/A*_search_algorithm">&#x4E00;&#x79CD;*</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/B*">B *</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Backtracking">&#x56DE;&#x6EAF;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Beam_search">&#x5149;&#x675F;</a>
          </li>
          <li>&#x8D1D;&#x5C14;&#x66FC;&#xB7;&#x798F;&#x7279;</li>
          <li><a href="https://en.wikipedia.org/wiki/Best-first_search">&#x6700;&#x4F73;&#x7B2C;&#x4E00;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Bidirectional_search">&#x53CC;&#x5411;&#x7684;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Bor%C5%AFvka%27s_algorithm">&#x535A;&#x5C14;&#x592B;&#x5361;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Branch_and_bound">&#x5206;&#x652F;&#x5B9A;&#x754C;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Breadth-first_search">BFS</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/British_Museum_algorithm">&#x82F1;&#x56FD;&#x535A;&#x7269;&#x9986;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/D*">D *</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Depth-first_search">DFS</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm">&#x8FEA;&#x514B;&#x65AF;&#x7279;&#x62C9;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Edmonds%27_algorithm">&#x57C3;&#x5FB7;&#x8499;&#x5179;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Floyd%E2%80%93Warshall_algorithm">&#x5F17;&#x6D1B;&#x4F0A;&#x5FB7;&#xB7;&#x6C83;&#x6B47;&#x5C14;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Fringe_search">&#x8FB9;&#x7F18;&#x641C;&#x7D22;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Hill_climbing">&#x722C;&#x5C71;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Iterative_deepening_A*">IDA *</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Iterative_deepening_depth-first_search">&#x8FED;&#x4EE3;&#x52A0;&#x6DF1;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Johnson%27s_algorithm">&#x7EA6;&#x7FF0;&#x900A;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Jump_point_search">&#x8DF3;&#x8DC3;&#x70B9;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Kruskal%27s_algorithm">&#x514B;&#x9C81;&#x65AF;&#x5361;&#x5C14;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Lexicographic_breadth-first_search">&#x8BCD;&#x5178;BFS</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Lifelong_Planning_A*">LPA *</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Prim%27s_algorithm">&#x539F;&#x59CB;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/SMA*">&#x9AD8;&#x4E2D;*</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Shortest_Path_Faster_Algorithm">SPFA</a>
          </li>
        </ul>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| 清单 |
| :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">
        <ul>
          <li><a href="https://en.wikipedia.org/wiki/Category:Graph_algorithms">&#x56FE;&#x7B97;&#x6CD5;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Category:Search_algorithms">&#x641C;&#x7D22;&#x7B97;&#x6CD5;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/List_of_algorithms#Graph_algorithms">&#x56FE;&#x7B97;&#x6CD5;&#x5217;&#x8868;</a>
          </li>
        </ul>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

| 相关话题 |
| :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">
        <ul>
          <li><a href="https://en.wikipedia.org/wiki/Dynamic_programming">&#x52A8;&#x6001;&#x7F16;&#x7A0B;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Graph_traversal">&#x56FE;&#x904D;&#x5386;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Tree_traversal">&#x6811;&#x904D;&#x5386;</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Search_game">&#x641C;&#x7D22;&#x6E38;&#x620F;</a>
          </li>
        </ul>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

<table>
  <thead>
    <tr>
      <th style="text-align:left">
        <ul>
          <li><a href="https://en.wikipedia.org/wiki/Template:Graph_search_algorithm">v</a>
          </li>
          <li><a href="https://en.wikipedia.org/wiki/Template_talk:Graph_search_algorithm">&#x164;</a>
          </li>
          <li><a href="https://en.wikipedia.org/w/index.php?title=Template:Graph_search_algorithm&amp;action=edit">&#xCB;</a>
          </li>
        </ul>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>

在图形的各种应用中发现了负边缘权重，因此该算法很有用。[\[3\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-FOOTNOTESedgewick2002-3) 如果图形包含从源头可以到达的“负循环”（即边的总和为负值的[循环](https://en.wikipedia.org/wiki/Cycle_%28graph_theory%29)），则没有最便宜的路径：在负循环上有点的任何路径都可以绕负周期再[走一圈](https://en.wikipedia.org/wiki/Walk_%28graph_theory%29)，使价格更便宜。在这种情况下，Bellman-Ford算法可以检测并报告负循环。[\[1\] ](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-Bang-1)[\[4\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-FOOTNOTEKleinbergTardos2006-4)

### 内容 <a id="mw-toc-heading"></a>

* [1种算法](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Algorithm)
* [2正确性证明](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Proof_of_correctness)
* [3寻找负周期](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Finding_negative_cycles)
* [4路由应用](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Applications_in_routing)
* [5项改进](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Improvements)
* [6琐事](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Trivia)
* [7笔记](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Notes)
* [8参考](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#References)
  * [8.1原始资料](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Original_sources)
  * [8.2次要来源](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#Secondary_sources)

### 算法\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=1)\]

[![](https://upload.wikimedia.org/wikipedia/commons/thumb/8/85/Bellman-Ford_worst-case_example.svg/220px-Bellman-Ford_worst-case_example.svg.png)](https://en.wikipedia.org/wiki/File:Bellman-Ford_worst-case_example.svg)在此示例图中，假设A是源，并且以从右到左的最差顺序处理边缘，则需要使用\| V \| -1或4次迭代，以使距离估计收敛。相反，如果按从左到右的最佳顺序处理边缘，则算法将在一次迭代中收敛。

像[Dijkstra的算法](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)一样，Bellman-Ford通过[松弛进行](https://en.wikipedia.org/wiki/Relaxation_%28iterative_method%29)，其中将正确距离的近似值替换为更好的近似值，直到最终找到解。在这两种算法中，到每个顶点的近似距离始终是真实距离的高估，并被其旧值的最小值和新找到的路径的长度所替代。但是，Dijkstra的算法使用[优先级队列](https://en.wikipedia.org/wiki/Priority_queue)来[贪婪地](https://en.wikipedia.org/wiki/Greedy_algorithm)选择尚未处理的最接近的顶点，并在其所有出站边缘执行此松弛过程。相比之下，Bellman-Ford算法只是放松所有边缘，然后执行此操作{ displaystyle \| V \| -1}![\| V \| -1](https://wikimedia.org/api/rest_v1/media/math/render/svg/6407482f919e956e1d22eb304c73a841e395e436) 时间，在哪里 { displaystyle \| V \|}![\| V \|](https://wikimedia.org/api/rest_v1/media/math/render/svg/9ddcffc28643ac01a14dd0fb32c3157859e365a7)是图中的顶点数。在每个重复中，具有正确计算出的距离的顶点数量会增加，由此得出的结论是所有顶点最终都将具有正确的距离。与Dijkstra相比，此方法允许将Bellman-Ford算法应用于更广泛的输入类别。

贝尔曼-福特参加 { displaystyle O（\| V \|  cdot \| E \|）}![O&#xFF08;\| V \|  cdot \| E \|&#xFF09;](https://wikimedia.org/api/rest_v1/media/math/render/svg/93b30ae8ec84ab14193f0b6a384c39e796c80545) [时间](https://en.wikipedia.org/wiki/Big_O_notation)，地点{ displaystyle \| V \|}![\| V \|](https://wikimedia.org/api/rest_v1/media/math/render/svg/9ddcffc28643ac01a14dd0fb32c3157859e365a7) 和 { displaystyle \| E \|}![\| E \|](https://wikimedia.org/api/rest_v1/media/math/render/svg/d8c2b9637808cf805d411190b4ae017dbd4ef8d8) 分别是顶点和边的数量。

```text
function BellmanFord(list vertices, list edges, vertex source) is
    ::distance[], predecessor[]

    // This implementation takes in a graph, represented as
    // lists of vertices and edges, and fills two arrays
    // (distance and predecessor) about the shortest path
    // from the source to each vertex

    // Step 1: initialize graph
    for each vertex v in vertices do
        distance[v] := inf             // Initialize the distance to all vertices to infinity
        predecessor[v] := null         // And having a null predecessor

    distance[source] := 0              // The distance from the source to itself is, of course, zero

    // Step 2: relax edges repeatedly
    for i from 1 to size(vertices)−1 do //just |V|−1 repetitions; i is never referenced
        for each edge (u, v) with weight w in edges do
            if distance[u] + w < distance[v] then
                distance[v] := distance[u] + w
                predecessor[v] := u

    // Step 3: check for negative-weight cycles
    for each edge (u, v) with weight w in edges do
        if distance[u] + w < distance[v] then
            error "Graph contains a negative-weight cycle"

    return distance[], predecessor[]
```

简而言之，该算法将到源的距离初始化为0，将所有其他节点的距离初始化为无穷大。然后，对于所有边缘，如果可以通过抓住边缘来缩短到目的地的距离，则该距离将更新为新的较低值。在每次迭代中我其边缘扫描时，算法找到至多长度的所有最短路径我边缘（和可能的一些路径长于我边缘）。由于没有循环的可能的最长路径是{ displaystyle \| V \| -1}![\| V \| -1](https://wikimedia.org/api/rest_v1/media/math/render/svg/6407482f919e956e1d22eb304c73a841e395e436) 边缘，必须扫描边缘 { displaystyle \| V \| -1}![\| V \| -1](https://wikimedia.org/api/rest_v1/media/math/render/svg/6407482f919e956e1d22eb304c73a841e395e436)时间以确保找到所有节点的最短路径。对所有边缘进行最终扫描，如果更新了任何距离，则为长度路径{ displaystyle \| V \|}![\| V \|](https://wikimedia.org/api/rest_v1/media/math/render/svg/9ddcffc28643ac01a14dd0fb32c3157859e365a7) 已发现只有在图形中至少存在一个负循环时才会出现边沿。

### 正确性证明\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=2)\]

| [![](https://upload.wikimedia.org/wikipedia/en/thumb/9/99/Question_book-new.svg/50px-Question_book-new.svg.png)](https://en.wikipedia.org/wiki/File:Question_book-new.svg) | 本节**未**[**引用**](https://en.wikipedia.org/wiki/Wikipedia:Citing_sources)**任何**[**资料**](https://en.wikipedia.org/wiki/Wikipedia:Verifiability)。请通过[在可靠来源中添加引文来](https://en.wikipedia.org/wiki/Help:Introduction_to_referencing_with_Wiki_Markup/1)帮助[改进本节](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit)。未采购的材料可能受到挑战并被[清除](https://en.wikipedia.org/wiki/Wikipedia:Verifiability#Burden_of_evidence)。查找来源：[“贝尔曼福特算法”](https://www.google.com/search?as_eq=wikipedia&q=%22Bellman%E2%80%93Ford+algorithm%22)  –  [新闻](https://www.google.com/search?tbm=nws&q=%22Bellman%E2%80%93Ford+algorithm%22+-wikipedia)**·** [报纸](https://www.google.com/search?&q=%22Bellman%E2%80%93Ford+algorithm%22+site:news.google.com/newspapers&source=newspapers)**·** [书籍](https://www.google.com/search?tbs=bks:1&q=%22Bellman%E2%80%93Ford+algorithm%22+-wikipedia)**·** [学者](https://scholar.google.com/scholar?q=%22Bellman%E2%80%93Ford+algorithm%22)**·** [JSTOR](https://www.jstor.org/action/doBasicSearch?Query=%22Bellman%E2%80%93Ford+algorithm%22&acc=on&wc=on)          （2019年3月）（[了解如何以及何时删除此模板消息](https://en.wikipedia.org/wiki/Help:Maintenance_template_removal)） |
| :--- | :--- |


该算法的正确性可以通过[归纳证明](https://en.wikipedia.org/wiki/Mathematical_induction)：

**引理**。在我重复for循环之后，

* 如果Distance（u）不是无穷大，则它等于从s到u的某些路径的长度；和
* 如果存在从s到u的路径（最多i个边缘），那么Distance（u）最多是从s到u的最多i个边缘的最短路径的长度。

**证明**。对于异步的基本情况，考虑`i=0`和之前的那一刻为首次执行循环。然后，对于源顶点`source.distance = 0`，这是正确的。对于其他顶点u，这也是正确的，因为从源到u的路径都不存在0条边。 `u.distance =` **`infinity`**

对于归纳案例，我们首先证明第一部分。考虑一下顶点距离更新为的时刻 `v.distance := u.distance + uv.weight`。通过归纳假设，`u.distance`是从源到u的某些路径的长度。然后`u.distance + uv.weight`是从源到v的路径的长度，该路径的长度沿着从源到u的路径 ，然后到v。

对于第二部分，请考虑从源到v的最短路径P（可能有不止一条），最多具有i个边缘。令u为该路径上v之前的最后一个顶点。然后，从路径的一部分来源，以ü是从最短路径源到ü至多I-1的边缘，因为如果它不是，那么就必须有一些严格的短路径源到ü最多与I- 1条边，然后我们可以将边uv附加到此路径，以获得一条最多具有i的边界严格小于P－矛盾。通过归纳假设，`u.distance`在i -1迭代之后，最多是该路径从源到u的长度。因此，`uv.weight + u.distance`最大为P的长度。在第i 次迭代中，`v.distance`与进行比较`uv.weight + u.distance`，如果`uv.weight + u.distance`较小，则设置为等于。因此，在i次迭代之后，`v.distance`最多为P的长度，即，从源到v的最短路径的长度最多为i个边缘。

如果没有负权重循环，则每个最短路径最多会访问每个顶点一次，因此在步骤3中无法进行进一步的改进。相反，假设无法进行任何改进。然后对于顶点v \[0\]，...，v \[ k -1\]的任何循环，

`v[i].distance <= v[i-1 (mod k)].distance + v[i-1 (mod k)]v[i].weight`

围绕循环进行总结，v \[ i \] .distance和v \[ i -1（mod k）\]。distance项抵消，从而使

`0 <= sum from 1 to k of v[i-1 (mod k)]v[i].weight`

即，每个周期的权重均为非负数。

### 寻找负周期\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=3)\]

当使用该算法查找最短路径时，存在负循环是一个问题，从而阻止了该算法找到正确的答案。但是，由于它会在找到负循环时终止，因此Bellman-Ford算法可用于寻求该目标的应用程序，例如在[网络流量](https://en.wikipedia.org/wiki/Flow_network)分析中的[循环取消](https://en.wikipedia.org/w/index.php?title=Cycle-cancelling&action=edit&redlink=1)技术中。[\[1\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-Bang-1)

### 路由中的应用\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=4)\]

Bellman-Ford算法的分布式变体用于[距离矢量路由协议](https://en.wikipedia.org/wiki/Distance-vector_routing_protocol)，例如[路由信息协议](https://en.wikipedia.org/wiki/Routing_Information_Protocol)（RIP）。该算法是分布式的，因为它涉及[自治系统中](https://en.wikipedia.org/wiki/Autonomous_system_%28Internet%29)的多个节点（路由器），[自治系统](https://en.wikipedia.org/wiki/Autonomous_system_%28Internet%29)是ISP通常拥有的IP网络的集合。它包括以下步骤：

1. 每个节点计算自身与AS中所有其他节点之间的距离，并将此信息存储为表格。
2. 每个节点将其表发送到所有相邻节点。
3. 当节点从其邻居接收到距离表时，它会计算到所有其他节点的最短路径，并更新其自己的表以反映所有更改。

在这种情况下，Bellman-Ford算法的主要缺点如下：

* 它的伸缩性不好。
* 由于更新是逐节点传播的，因此无法快速反映[网络拓扑的](https://en.wikipedia.org/wiki/Network_topology)变化。
* 如果链路或节点故障使某个节点无法从其他一组节点到达某个节点，则[计数到无穷大](https://en.wikipedia.org/wiki/Count_to_infinity#Count-to-infinity_problem)，这些节点可能会永远花时间逐渐增加其对与节点的距离的估计，并且与此同时可能存在路由环路。

### 改进\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=5)\]

通过观察以下事实，可以在实践中（尽管不是在最坏的情况下）改进Bellman-Ford算法：如果算法主循环的迭代在不进行任何更改的情况下终止，则可以立即终止该算法，因为随后的迭代将不再进行任何更改。在这种提前终止条件下，在某些情况下，主循环使用的数量可能少于\| \|。V \| − 1次迭代，即使算法的最坏情况保持不变。

[Yen（1970）](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFYen1970)对没有负权重循环的图描述了Bellman-Ford算法的另外两个改进。再次，虽然在实践中使算法更快，但他们并没有改变其算法。{ displaystyle O（\| V \|  cdot \| E \|）}![O&#xFF08;\| V \|  cdot \| E \|&#xFF09;](https://wikimedia.org/api/rest_v1/media/math/render/svg/93b30ae8ec84ab14193f0b6a384c39e796c80545)最坏的情况是时间限制。他的第一项改进减少了算法每次迭代中需要执行的松弛步骤的数量。如果顶点v的距离值自上次松弛v以来没有变化，则无需再次使v之外的边缘松弛。这样，随着具有正确距离值的顶点数量的增加，在每次迭代中需要放松的输出边缘的数量会减少，从而为[密集图](https://en.wikipedia.org/wiki/Dense_graph)节省了时间常数。

颜的第二个改进是首先在所有顶点上分配一些任意的线性顺序，然后将所有边的集合划分为两个子集。所述第一子集，ê ˚F，包含所有边缘（v 我，v Ĵ），使得我 &lt; Ĵ ; 第二个E b包含边（v i，v j），使得i &gt; j。每个顶点按v 1，v 2，...，v \|的顺序访问。V \|，从E f的那个顶点放宽每个输出边缘。然后按v \| \|的顺序访问每个顶点。V \| ，v \| V \| −1，...，v 1，从E b中的那个顶点放宽每个输出边缘。在第一个迭代之后，算法主循环的每次迭代都会在其松弛距离与正确的最短路径距离匹配的一组边缘中至少添加两个边缘：一个来自E f，一个来自E b。此修改从\|减少了算法主循环的最坏情况迭代次数。V\| − 1至{ displaystyle \| V \| / 2}![\| V \| / 2](https://wikimedia.org/api/rest_v1/media/math/render/svg/969159a4606100e8bf46319874300f27fc64c9d9)。[\[5\] ](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-5)[\[6\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-Sedweb-6)

[Bannister＆Eppstein（2012）的](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFBannisterEppstein2012)另一项改进是用[随机置换](https://en.wikipedia.org/wiki/Random_permutation)代替了日元第二次改进中所用顶点的任意线性顺序。这种变化使Yen的改进变得最糟（最短路径的边缘在两个子集E f和E b之间严格交替）极不可能发生。使用随机排列的顶点顺序，主循环中所需的[预期](https://en.wikipedia.org/wiki/Expected_value)迭代次数最多为{ displaystyle \| V \| / 3}![\| V \| / 3](https://wikimedia.org/api/rest_v1/media/math/render/svg/e464851c4b44de4d198e82c9aae50766e3b6a88c)。[\[6\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-Sedweb-6)

### 琐事\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=6)\]

在中国，还增加了一个先入先出队列的Bellman-Ford算法，被称为算法[SPFA](https://en.wikipedia.org/wiki/SPFA)，由爱德华·摩尔在1959年，1994年出版，重新发现了Fanding段，深受谁参加学生[国家省](https://en.wikipedia.org/w/index.php?title=National_Olympiad_in_Informatics_in_Provinces&action=edit&redlink=1) \[ [zh](https://zh.wikipedia.org/wiki/%E5%85%A8%E5%9B%BD%E9%9D%92%E5%B0%91%E5%B9%B4%E4%BF%A1%E6%81%AF%E5%AD%A6%E5%A5%A5%E6%9E%97%E5%8C%B9%E5%85%8B%E8%81%94%E8%B5%9B) \] [省信息奥林匹克竞赛](https://en.wikipedia.org/w/index.php?title=National_Olympiad_in_Informatics_in_Provinces&action=edit&redlink=1)和[国际大学编程竞赛](https://en.wikipedia.org/wiki/International_Collegiate_Programming_Contest)。[\[7\]](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_note-duan-7)

### 笔记\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=7)\]

1. ^ [跳至：**a** ](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Bang_1-0)[**b** ](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Bang_1-1)[**c** ](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Bang_1-2)[**d**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Bang_1-3) [Bang-Jensen＆Gutin（2000）](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFBang-JensenGutin2000)
2. [**^**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Schrijver_2-0) [作者（2005）](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFSchrijver2005)
3. [**^**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-FOOTNOTESedgewick2002_3-0) [Sedgewick（2002）](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFSedgewick2002)。
4. [**^**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-FOOTNOTEKleinbergTardos2006_4-0) [Kleinberg＆Tardos（2006）](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#CITEREFKleinbergTardos2006)。
5. [**^**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-5) Cormen等人，第二版，问题24-1，第614-615页。
6. ^ [跳转到：**一个**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Sedweb_6-0) [**b**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-Sedweb_6-1) 见塞奇威克的[幅练习](http://algs4.cs.princeton.edu/44sp/)为算法。，第4版，演习5和12（检索二○一三年一月三十○日）。
7. [**^**](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm#cite_ref-duan_7-0) Duan, Fanding \(1994\), ["关于最短路径的SPFA快速算法"](http://wenku.baidu.com/view/3b8c5d778e9951e79a892705.html), Journal of Southwest Jiaotong University, **29** \(2\): 207–212

### 参考\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=8)\]

#### 原始资料\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=9)\]

* Shimbel，A.（1955年）。通信网络中的结构。信息网络研讨会论文集。纽约，纽约：布鲁克林理工学院的理工出版社。第199–203页。
* [理查德·贝尔曼](https://en.wikipedia.org/wiki/Richard_Bellman)（1958）。“关于路由问题”。应用数学季刊。**16**：87-90。[MR ](https://en.wikipedia.org/wiki/Mathematical_Reviews) [0102435](https://www.ams.org/mathscinet-getitem?mr=0102435)。
* [福特，小莱斯特·R。](https://en.wikipedia.org/wiki/L._R._Ford_Jr.)（1956年8月14日）。[网络流理论](http://www.rand.org/pubs/papers/P923.html)。论文P-923。加利福尼亚州圣莫尼卡：兰德公司。
* [摩尔，爱德华·F](https://en.wikipedia.org/wiki/Edward_F._Moore)（1959）。穿过迷宫的最短路径。程序 国际交流。座谈会。转换理论，1957年，第二部分。马萨诸塞州剑桥市：哈佛大学。按。第285–292页。[MR ](https://en.wikipedia.org/wiki/Mathematical_Reviews) [0114710](https://www.ams.org/mathscinet-getitem?mr=0114710)。
* 颜金Y（1970）。“在通用网络中找到从所有源节点到给定目的地的最短路径的算法”。应用数学季刊。**27**：526–530。[MR ](https://en.wikipedia.org/wiki/Mathematical_Reviews) [0253822](https://www.ams.org/mathscinet-getitem?mr=0253822)。
* 密西根州班尼斯特；[Eppstein，D.](https://en.wikipedia.org/wiki/David_Eppstein)（2012年）。[Bellman-Ford算法](https://arxiv.org/pdf/1111.5414.pdf) （PDF）的[随机加速](https://arxiv.org/pdf/1111.5414.pdf)。分析算法和组合学（ANALCO12），日本京都。第41–47页。[arXiv](https://en.wikipedia.org/wiki/ArXiv)：[1111.5414](https://arxiv.org/abs/1111.5414)。[Bibcode](https://en.wikipedia.org/wiki/Bibcode)：[2011arXiv1111.5414B](https://ui.adsabs.harvard.edu/abs/2011arXiv1111.5414B)。

#### 次要来源\[ [编辑](https://en.wikipedia.org/w/index.php?title=Bellman%E2%80%93Ford_algorithm&action=edit&section=10)\]

* Bang-Jensen，Jørgen; 古丁，格雷戈里（2000）。“第2.3.4节：Bellman-Ford-Moore算法”。[图：理论，算法和应用](http://www.cs.rhul.ac.uk/books/dbook/)（第一版）。[书号](https://en.wikipedia.org/wiki/International_Standard_Book_Number) [978-1-84800-997-4](https://en.wikipedia.org/wiki/Special:BookSources/978-1-84800-997-4)。
* Schrijver，Alexander（2005）。[“关于组合优化的历史（至1960年）” ](http://homepages.cwi.nl/~lex/files/histco.pdf)（PDF）。离散优化手册。爱思唯尔：1-68。
* [Cormen，托马斯H](https://en.wikipedia.org/wiki/Thomas_H._Cormen) ; [Leiserson，查尔斯·E](https://en.wikipedia.org/wiki/Charles_E._Leiserson) ; [Rivest，Ronald L. ](https://en.wikipedia.org/wiki/Ron_Rivest)[算法简介](https://en.wikipedia.org/wiki/Introduction_to_Algorithms)。麻省理工学院出版社和麦格劳-希尔。， 第二版。麻省理工学院出版社和麦格劳-希尔，2001年[ISBN ](https://en.wikipedia.org/wiki/International_Standard_Book_Number)[0-262-03293-7](https://en.wikipedia.org/wiki/Special:BookSources/0-262-03293-7)。第24.1节：Bellman-Ford算法，第588-592页。问题24-1，第614–615页。第三版。麻省理工学院出版社，2009年。[ISBN ](https://en.wikipedia.org/wiki/International_Standard_Book_Number)[978-0-262-53305-8](https://en.wikipedia.org/wiki/Special:BookSources/978-0-262-53305-8)。第24.1节：Bellman-Ford算法，第651-655页。  
* Heineman，乔治·T。加里·波利斯（Pollice，Gary）；斯坦利·瑟尔科（2008）。“第6章：图形算法”。简而言之的算法。[奥赖利媒体](https://en.wikipedia.org/wiki/O%27Reilly_Media)。第160–164页。[书号](https://en.wikipedia.org/wiki/International_Standard_Book_Number) [978-0-596-51624-6](https://en.wikipedia.org/wiki/Special:BookSources/978-0-596-51624-6)。
* [乔恩·克莱恩伯格](https://en.wikipedia.org/wiki/Jon_Kleinberg)；[塔多斯·埃瓦](https://en.wikipedia.org/wiki/%C3%89va_Tardos)（2006）。算法设计。纽约：培生教育有限公司
* [Sedgewick，Robert](https://en.wikipedia.org/wiki/Robert_Sedgewick_%28computer_scientist%29)（2002）。“第21.7节：负边权重”。[Java中的算法](https://web.archive.org/web/20080531142256/http://safari.oreilly.com/0201361213/ch21lev1sec7)（第3版）。[书号](https://en.wikipedia.org/wiki/International_Standard_Book_Number) [0-201-36121-3](https://en.wikipedia.org/wiki/Special:BookSources/0-201-36121-3)。（[原始](http://safari.oreilly.com/0201361213/ch21lev1sec7)内容存档于2008-05-31）。检索2007-05-28。

[分类](https://en.wikipedia.org/wiki/Help:Category)：

* [图算法](https://en.wikipedia.org/wiki/Category:Graph_algorithms)
* [多项式时间问题](https://en.wikipedia.org/wiki/Category:Polynomial-time_problems)
* [动态编程](https://en.wikipedia.org/wiki/Category:Dynamic_programming)


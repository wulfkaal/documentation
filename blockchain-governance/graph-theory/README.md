# Graph Theory

Technically the forum on Semada is a weighted, directed, acyclic graph \(​WDAG​\), and the valuation of the posts is a network flow. We review these definitions next.

A ​graph​ is a collection of points, called ​vertices​, with optional connections between vertices, called ​edges​. The vertices of our graph are the posts to the forum. The edges are citations directed from one post \(the ​referrer​\) to another \(the ​reference​\). The edges give the graph direction, since references always point backward in time. Since there can be no time loops of references, the graph has no cycles, so it is ​acyclic​. All in all, the forum is a directed acyclic graph \(DAG\).

![](../../.gitbook/assets/image%20%287%29.png)

Our job is to weight the DAG and stipulate the weight’s meaning. To do this, we assign a number to each post \(vertex\), indicating its importance in contributing to the mission of the respective DAO. This number determines the value of each sem token created for that post. The author of any post assigns numbers to each of their references \(edges\) to indicate how important the reference post was in helping to make their contribution. How these weights are assigned and how the weights of edges affect the weights of vertices is a crucial factor in determining the reward structure and ultimately the values that are encouraged in the evolution of the company.

There are many families of choices for weighting the value of posts through references. To illustrate the idea, we detail an extremely basic example next. 




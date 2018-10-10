# Evolutionary Blockchain Governance Protocol

The Semada protocol uses a weighted directed acyclic graph for a precedent system and DAO governance.  


A graph is a collection of points, called vertices, with optional connections between vertices, called edges. The vertices of our graph are the posts to the forum. The edges are citations directed from one post \(the referrer\) to another \(the reference\). The edges give the graph direction, since references always point backward in time. Since there can be no time loops of references, the graph has no cycles, so it is acyclic. All in all, the forum is a directed acyclic graph \(DAG\).

DAO Governance Via Weighted Directed Acyclical Graphs

![](https://lh5.googleusercontent.com/FnxCQh4G0ivutnfG-iCRdO_V80NdF_Yjg6DwHIdVThUaC3HrzF-jdFT58oW_DFLCMsegZQuaAuy-hYiG9aTBgqvn61BsSbgHDS9hZV--87Dv3PIfS34HnwVJTv4RzqgtCzK8T4cy)

Figure 9: Weighted Directed Acyclical Graphs.

DAO Governance Precedent System via Weighted DAG

![](https://lh6.googleusercontent.com/utS13OmwimUICVb70_GV8IDal_BLN6INMnEckhbDKYDXfLI45LnUOVRMFZvB5EbGzoG0Cjoh9GvJNxXIKpH_xn---Y7ob0jccdK80wEqiVPHevZWwcxgb5IX8j1frZVeCy53pNMQ)

Figure 10: Weighted DAG Precedent System.  


In the Semada Protocol, evolutionary DAO governance is enable by the Weighted DAG precedent system. As Figure 10 above demonstrates, more reputation weight and salaries are allocated to posts on the Semada Forum that get continuously referenced by other posts. As a precedent dissipates over time, new precedence in the Semada Forum emerge naturally to replace older precedent. This is the essence of the evolutionary nature of the platform. As a matter of fact,  entire expertise tags and DAOs on the Semada platforms can emerge and be replaced over time with new and improved systems naturally within the existing architecture of the platform.

  
  
2.2 Weights and rewards

The basic process of creating and validating posts which document contributions to an organization is explained above. Our next task is to analyze the many options that arise for weighting references, and what organizational values and goals are incentivized by the consequent reward structure.

#### 2.2.1 Details: graph theory description of the company

To specify this weighting structure a bit more rigorously, we introduce some technical jargon that may sound complicated in the beginning, but there is no deep mathematics involved. Technically the forum is a weighted, directed, acyclic graph \(**WDAG**\), and the valuation of the posts is a network flow. We review these definitions next.

A **graph** is a collection of points, called **vertices**, with optional connections between vertices, called **edges**. The vertices of our graph are the posts to the forum. The edges are citations directed from one post \(the **referrer**\) to another \(the **reference**\). The edges give the graph direction, since references always point backward in time. Since there can be no time loops of references, the graph has no cycles, so it is **acyclic**. All in all, the forum is a directed acyclic graph \(DAG\).

![](../.gitbook/assets/image%20%287%29.png)

Figure 1: Graph definitions

Our job is to weight the DAG and stipulate the weight’s meaning. To do this, we assign a number to each post \(vertex\), indicating its importance in contributing to the mission of the respective DAO. This number determines the value of each sem token created for that post. The author of any post assigns numbers to each of their references \(edges\) to indicate how important the reference post was in helping to make their contribution. How these weights are assigned and how the weights of edges affect the weights of vertices is a crucial factor in determining the reward structure and ultimately the values that are encouraged in the evolution of the company.

There are many families of choices for weighting the value of posts through references. To illustrate the idea, we detail an extremely basic example next, before analyzing more general options in §3.

#### 2.2.2 A toy model of reference weights

Each post ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image004.jpg) has a different value ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image006.jpg), depending on a number of factors. In this first toy model for valuating posts, we specify a number of choices that will later be opened to variation depending on the needs of each particular DAO. First, a post mints a number of sem tokens proportional to the fee that is associated with it. For this example we mint 1 token per dollar, so ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image008.jpg). Secondly, a post is weighted by the amount of approval it initially receives, i.e., the margin of success in the voting pool. Finally the post changes value due to any references it later receives.

In this example, posters may reward or punish more than one previous post with a reference and a weight number ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image010.jpg) chosen between ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image012.jpg) and ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image014.jpg), where ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image016.jpg) means their post is in agreement with the reference and ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image018.jpg) means their post is opposed. Thus references become the weighted edges of the forum graph. Then to update the value of an older post, we simply sum up all of its referrers’ values multiplied by the weights.

![](../.gitbook/assets/image%20%284%29.png)

Figure 2:WDAG and network value flow

To be very specific, so that a programmer could implement this scheme, we stipulate the following notation.

**Post valuation algorithm.** Denote the posts ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg) numbered chronologically for ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image024.jpg) where ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image026.jpg) is the newest post. Denote the following symbols based on ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)

1\)    ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image029.jpg) “the weight from referrer ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image031.jpg) to reference ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)” where

●    ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image034.jpg)

●    ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image036.jpg) for ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image038.jpg) and 

●    ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image040.jpg)

![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image042.jpg)“total value of ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image045.jpg) with  
 ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image047.jpg)

2\)     where we define

                 i.      ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image049.jpg)“number of upvotes on ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”

                ii.      ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image052.jpg)“number of downvotes on ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”

               iii.      ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image055.jpg)“number of active voters during the pool for ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”

               iv.      ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image058.jpg)“number of tokens minted for ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”

                v.      ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image061.jpg)“initial value of ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg)”:=![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image064.jpg) 

The number ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image066.jpg) represents the number of active voters, determined by whether they have voted within the last month. Then ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image068.jpg) is the number of sem tokens associated with the post ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg). Each member who staked tokens on the winning side of the initial validation pool shares the ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image068.jpg) tokens proportionally, splits the staked tokens which were lost, and receives a reputation-weighted salary based on their total holdings. New positive references add more newly minted tokens which are shared proportionally with the original participants; new negative references burn tokens proportionally.

#### 2.2.3 Comments on the toy model

With this choice of valuating ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg) according to the recursive formula given for ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image068.jpg) in 2\) above, we are specifying that

1. Posts which were initially controversial are initially worth less according to the term ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image074.jpg) since in that case ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image076.jpg). This option favors harmony and consensus since unanimous votes generate more rewards, and so discourages active debate on contentious issues.
2. References add value according to their weight via the term ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image078.jpg) which allows posts to eternally rise or fall in sem influence. This option favors precedence and rewards long-term contributions. Bounding the weights ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image080.jpg) with ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image082.jpg) would limit the importance of precedence and protocol development, instead encouraging off-chain work by favoring new work-evidence posts as a more efficient means to gain power.
3. ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image040.jpg) means posts ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image031.jpg) can only give total references to past posts ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg) equal to their own value. References with the highest possible weight ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image087.jpg) confer value equal to the post ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image031.jpg) making the reference; chains of such references multiply the effect. This option gives power to quickly reward or punish older posts, but is less stable than if we limited the sum of absolute weights to a smaller value than ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image014.jpg).
4. Burned tokens cannot be regained in case the referring posts which destroyed their value are eventually overturned themselves. A slightly more complicated protocol would keep track of all the tokens created during a post, never allowing them to be burned, and keep a separate number determining the value of the token which is subject to change.
5. If a post  ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg) changes value by being newly referenced, all posts that ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image022.jpg) references will also change value; so the value of every post is eternally dynamic.
6. Notice the matrix ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image093.jpg) is upper triangular, since posts may only reference past posts. This makes the calculation of ![](file:////Users/wulfkaal/Library/Group%20Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image068.jpg) much more efficient in Semada’s DAG than in a more general network \(e.g., Google’s PageRank algorithm\) which means the cost of running the algorithm on a distributed network such as Ethereum is not as prohibitive.  

All of the qualities described in these comments may be changed or even reversed with a different choice of parameters and valuation functions, as will be discussed in Chapter III.

### 2.3 Summary

The reason no centralized platform, such as Amazon or EBay, has been able to create meaningful and secure online reputation arises from game theory inevitabilities: if there is a single static protocol for deciding how a centralized “opponent” apportions power, the game theory Folk Theorems prove there is inevitably a strategy for gaming the system and corrupting the value of reputation. With the new opportunities that blockchain technology creates, decentralizing reputation and distributing it fairly, the members can be properly incentivized and empowered to police all actions.

In order to create a platform that gives its users such power through tokens which represent reputation we require the following:

1. **Domain specific expertise.** Semada mints separate types of reputation tokens for every separate type of expertise or DAO.
2. **The tokens must have a foundational meaning.** Semada mints tokens only in proportion to the fees that are added to the platform.
3. For security, **the tokens must enter fairly**. Tokens are distributed only after they are staked for and against a post and the bench of experts validates them.
4. For security from Sybil attacks, **all decisions are made by weighted votes**.
5. To prevent a centralized point of attack and to properly motivate all experts, all power is determined by sem holdings and **all fees sent to the platform are shared proportionally in sem-weighted salaries**. Since sem acquisition becomes the primary motivation instead of immediately fungible currency, the incentive is to improve the platform instead of exploiting platform-damaging arbitrage opportunities.
6. **The opportunity for review of reputation by referencing past actions**
   1. prevents long-term gaming strategies from the threat of loss of long-term valuable reputation
   2. motivates long-term platform improvement and development from the opportunity for revaluating such actions once they are proven to be successful.

Giving DAO members the ability to fairly apportion power in a variety of expertises lessens the danger of the principal-agent problem\[1\] and combats several tragedy-of-the-commons problems, such as non-representativeness and free-riding.  


\[1\] Eirik G. Furubotn & Rudolf Richter, Institutions and Economic Theory: The Contribution of the New Institutional Economics, University of Michigan Press, 2005.


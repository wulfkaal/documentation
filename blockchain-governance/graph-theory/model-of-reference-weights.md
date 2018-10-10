# Model of Reference Weights

Each post p has a different value t , depending on a number of factors. In this first toy model for valuating posts, we specify a number of choices that will later be opened to variation

depending on the needs of each particular DAO. First, a post mints a number of sem tokens proportional to the fee that is associated with it. For this example we mint 1 token per dollar, 

so c1 = 1 . Secondly, a post is weighted by the amount of approval it initially receives, i.e., the margin of success in the voting pool. Finally the post changes value due to any references it later receives.

In this example, posters may reward or punish more than one previous post with a reference and a weight number w chosen between − 1 and 1 , where w = 1 means their post is in agreement with the reference and w =− 1 means their post is opposed. Thus references become the weighted edges of the forum graph. Then to update the value of an older post, we simply sum up all of its referrers’ values multiplied by the weights.

![](../../.gitbook/assets/image%20%2829%29.png)

![](../../.gitbook/assets/image%20%2826%29.png)

With this choice of valuating pn according to the recursive formula given for tn in 2\) above, we are specifying that

1. Posts which were initially controversial are initially worth less according to the term vn since in that case vn≈0. This option favors harmony and consensus since unanimous votes generate more rewards, and so discourages active debate on contentious issues.
2. References add value according to their weight via the term ∑ wn,k tk which allows posts k

   to eternally rise or fall in sem influence. This option favors precedence and rewards long-term contributions. Bounding the weights wn,k≤b with 0≤b≪1 would limit the

   importance of precedence and protocol development, instead encouraging off-chain work by favoring new work-evidence posts as a more efficient means to gain power.

c. ∑n \|wn,k\|≤1 means posts pk can only give total references to past posts pn equal to their own value. References with the highest possible weight wn,k = 1 confer value equal to the post pk making the reference; chains of such references multiply the effect. This option gives power to quickly reward or punish older posts, but is less stable than if we limited the sum of absolute weights to a smaller value than 1.

1. Burned tokens cannot be regained in case the referring posts which destroyed their value are eventually overturned themselves. A slightly more complicated protocol would keep track of all the tokens created during a post, never allowing them to be burned, and keep a separate number determining the value of the token which is subject to change.
2. If a post pn changes value by being newly referenced, all posts that pn references will also change value; so the value of every post is eternally dynamic.
3. Notice the matrix wn,k is upper triangular, since posts may only reference past posts. This makes the calculation of tn much more efficient in Semada’s DAG than in a more general network \(e.g., Google’s PageRank algorithm\) which means the cost of running the algorithm on a distributed network such as Ethereum is not as prohibitive.

All of the qualities described in these comments may be changed or even reversed with a different choice of parameters and valuation functions


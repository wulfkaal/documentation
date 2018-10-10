# Calculations

## The price to purchase 51% of the sem tokens

Here we demonstrate the attack resistance of the platform by showing that in the absolute worst-case scenario, the price to corrupt the system from within is a minimum of twice the total historical fees added to the system. If any obvious protections are instituted, the price to corrupt grows steeply.

Consider the situation where the platform has a total of g0 sem tokens at time 0. We will refer to all these users as good-faith experts. Imagine a malicious group m wishes to purchase 51% of the total sem tokens with fees, either to profit from future transactions or to destroy trust in the particular expertise tag. Since only half of their fees are added as sem tokens for the malicious group, and the other half will be added to the existing good-faith actors it is difficult to achieve the malicious goal, even in this worst-case scenario.

Under the ​worst-case scenario​, we suppose there are no safeguards against joining as an expert—any fee of any size is automatically accepted in the validation pool, and resolved instantly with no time delays. Finally we assume no other users are adding any fees.

Under this scenario, the best strategy for the malicious group to gain sem tokens by paying fees is to make many micro-payments. In the same way that continuously-compounded interest is better than discrete interest at the same rate, micro-payments allow malicious users to profit off their own later fees once their earlier fees vest them with sem tokens.

Thus we assume the malicious group m will add a variable number n of fixed fees of size ∆x≪1 . Then the good faith experts will have

![](../../.gitbook/assets/image%20%288%29.png)

![](../../.gitbook/assets/image%20%2831%29.png)

Consequently the malicious group would need to invest an absolute minimum of 2 g0 , that is, double the total sem tokens of the system to gain 50% power in the system in order to outvote the rest of the good-faith experts in the validation pool.

We stress that the value of 2g0 is an extremely conservative lower bound. In practice, the investments would need to be discrete values, not continuous. This significantly raises the minimum corrupting investment, and significantly lengthens the time needed to gain 51% power. Also, in practice many other users will be paying fees besides the malicious group, especially if the malicious group is pumping fees into the system.

Assuming the malicious group does manage to take over the platform, the rest of the world would immediately see the unfair action that couldn’t be rectified by the good-faith actors, so the expertise tag would topple, losing its value. The malicious group would merely gain the \(fraction\) of the fee from one transaction. As long as any single fee is smaller than the total sem tokens, there is no incentive to game the system for fees.

The only other reason to act maliciously is to destroy the particular expertise. But then the 2 g0 invested becomes worthless. So the minimum cost at any time to topple the system is twice the total sem tokens—assuming you can simply buy sem tokens without limit or oversight.

Therefore as long as the fees are low compared to the sem token total, or if there is no competitor that is suffering by the platform’s existence by more than twice the total number of sem tokens, it’s not worth spending money to corrupt the system—it is more valuable to use the power to improve the platform.

Further, as fees are added, sem tokens are added, so it becomes more secure as time goes on, even assuming constant fees.

Further, if a malicious group wishes to strike, their best strategy is to strike immediately. Their corrupt sem tokens become less valuable if they don’t use them, as each new fee they didn’t add to the system adds to other peoples’ tokens, diminishing the value of older tokens. So even if there are many different malicious groups, if no single malicious group gains 51% control, the system cannot be corrupted to unfairly earn fees.

A malicious group is therefore limited to attempting to destroy the platform, by overwhelming it with fees. If that is happening, and there is a reasonable time-delay in resolving validation pools, then the incoming malicious fees would encourage other, non-colluding parties to invest as well. This would significantly slow the effort to gain 51% for the malicious group.

Specifically, assume the good-faith experts invest some constant fraction c of the malicious groups’ investment ∆x at each time. If c ≥ 1 then the malicious group will never gain more than 50% power. So assume 0 &lt; c &lt; 1. Then the equations become

![](../../.gitbook/assets/image%20%284%29.png)

![](../../.gitbook/assets/image%20%2823%29.png)

## Natural sem token inflation

In this section we illustrate the value of one sem token with a few calculations. This demonstrates the value of an investment in sem tokens in the platform without using its power to evaluate posts. The conclusion is that the economy is inflationary at equilibrium, which improves its security and discourages rent-seeking.

One sem token loses value if fees are constantly added in time.

If fees are being paid into an expertise tag at a constant rate of F \(t\) = r units per time, then the salary paid for one coin decreases in time. To see this, denote the total number of sem tokens in the tag at time t by T\(t\). The salary per token per unit time is S = F/T . However, since each fee token creates a new sem token, we have

![](../../.gitbook/assets/image%20%2810%29.png)

![](../../.gitbook/assets/image%20%285%29.png)

**Early sem tokens are more valuable than later tokens.** 

All sem tokens in a single expertise tag are equal at any given moment. However, assuming a steady state rate of fees, the payout for 1 year from inception is greater for tokens minted earlier, because later tokens are a smaller percentage of the total. Remember, new tokens are created with every fee paid into the platform, but never destroyed.

This may mean later experts have less motivation to join if fees paid into the system are at a steady state. To combat this, the bench may choose to change the exchange rate between fees and sem tokens to encourage new recruits.


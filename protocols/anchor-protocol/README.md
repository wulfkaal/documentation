# Anchor Protocol

Block propagation in the platform is facilitated by staking reputation, not a fungible currency as in PoS. Accordingly, the consensus algorithm is called Proof of Reputation \(PoR\). In the infrastructure, this PoR protocol is called the Anchor Protocol because it is the first use of the underlying voting algorithm. Moreover, staking in the Anchor Protocol means anchoring your reputation to a block. In other words, block producers anchor their reputation to a block, and if the block is invalid or cancelled out, their reputation depreciates.  


How to use reputation for block production and propagation.  


Core comparison:  


![](https://lh6.googleusercontent.com/OX7U119Sebjh8WLkrqbsSZcAeHicTXV1Jplj46RcTme2o9dtZnJcpLDeu0D3c4EUm6WBUACEHcNkduMhvOuWSKOVSygbnTvgZaFhnZT5Zvr3e7skW1S0ljjiWgefr4TUuWVEXCSJ)

Consider a variation::



![](https://lh5.googleusercontent.com/WhRPJ771W4vxBfFY0G2jQiXBq0aRXHK64AZiWCSoyLKFIVAEQKaJ_3cRsZnL_hPZBBmeiF4Bi4VMPQ9IaPcLXlZ5baLk6y4Gm5yBUPfBSzgQ2SjVzoJWlpGni9hyTMo1e5SahH2R)

Anyone with any Anchor tokens has the potential to be a block producer. The platform Core \(pseudo\) randomly selects the block producers weighted by their holdings, meaning if you have more reputation, as evidenced by the Anchor holdings, you are more likely to be selected. This gives anyone on the planet, at any time, the opportunity to be a block producer.  


Block production is scheduled ahead of time where a list of randomly selected block producers is selected weighted by their Anchortoken holdings in the specific DAO related to block production. When a block producer's time comes, they produce and publish the block, sending its reference and all fees included to the platform Core to open a validation pool \(betting pool\) where the other SEM Token holders can check the block is created according to protocol and vote accordingly. Consensus follows a slight variation on the GHOST protocol \(greedy heaviest observed subtree\) that bitcoin and Ethereum use for proof of work, meaning the subtree with the greatest weight of SEM Token-backed votes is canonical. Then all fees collected from the block of transactions are distributed in the reputation-weighted salary.  


So a successful block producer doesn't win the lottery with a great deal of fees if they are chosen, they win the lottery of half of a great deal of new reputation tokens if they are chosen while the rest of the members share the other half of newly minted reputation tokens for policing the block in the validation pool. This makes the whole system more stable \(salary of fungible fees is regular and predictable as opposed to winning the lottery\) and gives better incentives \(e.g., there is less reason to join a mining pool, since all fungible fees are already shared in proper proportion, so it is more decentralized\).  


Active participation is encouraged because new reputation tokens are minted in every validation pool for every block. So block production is strongly encouraged \(because a greater percentage of the new tokens are given to a successful producer\) and policing is gently encouraged \(you share in part of the new tokens with everyone who is active, which encourages activity but doesn't unstably slash non-participation \(which can be innocent if the network is down, etc.\)\).  


Producing bad blocks is slashed because the bad block producer will lose their availability stakes \(the tokens the producer staked to be considered for the random selection of block producers\) in the validation pool.  


The computing resources are whatever it takes to make a block \(no resources needed to hash mine\). Currently making a block is very easy for a laptop or even a good cellphone to do.  



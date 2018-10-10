---
description: This page explains the central elements of the Semada Voting Algorithm
---

# Semada Core

Semada is an autonomous decentralized platform for validating domain specific reputation. The main design goals of the Semada platform are to:

1. evaluate domain specific reputation across a wide variety of expertises
2. insure security, including resistance to Sybil attacks, tyranny of the majority, and 51%

   attacks

3. provide a minimal, robust core architecture which supports modular constructions for a

   wide range of use cases.

The key features are

1. a ​positive feedback loop which promotes productive cooperation between public and expert users
2. maximal freedom for experts in the creation of reputation verification protocols
3. complete autonomy—the economic structure is closed to off-domain influence; all power

   and fees are shared entirely by expert users, weighted by reputation

4. meritocracy—the platform supports anonymity, rewarding ability and productive

   contributions over personal identity.

The Semada platform creates a transparent, fair, and predictable system that facilitates certainty of outcomes, security, and efficiency. Society benefits from the advancement of justice and prevention of corruption on a global scale.





Semada core basics

While the core Semada architecture can be implemented on other types of infrastructure, Ethereum was chosen to host the first implementation, due to its decentralized, censorship-resistant, modular architecture and extensive developer adoption features.

The core Semada platform exposes five external functions:

1. Get list of expertises.
2. Get list of experts given an expertise.
3. Announce expert availability stake for random selection.
4. Add a validation request to Semada.
5. Vote on a validation request by staking expertise specific tokens.

The typical flow of events for a user interacting with Semada core is the following:

1. Public user Alice has some work which needs to be done that requires a certain expertise.
2. Alice searches the forum for solutions. An off-platform user interface which organizes

   the information of the forum suggests the appropriate expertises and smart contracting

   language for finding an expert in the system.

3.  Alice chooses a smart contract \(SC\), sends SC and the ETH fee to Semada.
4. Accessing the Semada platform, SC does the following:

   a\)  SC queries the Semada platform to get the list of all experts and their posted

   availability stakes from the chosen expertise.

   b\)  SC randomly chooses an expert, Bob. The random selection follows a weighted

   distribution determined by the posted availability stakes of the experts in the

   expertise.

   c\)  SC takes control of Bob’s availability stake.

   d\)  SC informs Bob of his selection and the work Alice requires to be done.

   e\)  Bob does the work for Alice off platform.

   f\)  Bob sends his evidence-of-work post to SC.

   g\)  In Bob’s \(pseudonymous\) name, SC sends Bob’ evidence-of-work post and

   Alice’s ETH fee to Semada.

5. The Semada platform distributes Alice’s ETH fee to the domain experts, proportionately,

   based on the amount of sub-tokens they own for that expertise

6. The platform mints new domain-specific sub-tokens, based on the amount of ETH sent

   and the exchange rate between ETH and the respective sub-token. \(Within each expertise,

   the bench decides the exchange rate. See §​9.1 Expert parameter maintenance​.\)

7. Validation pool opens. Half of the new tokens are staked for upvote and assigned to Bob. \(This is Bob’s payment for the work he’s done\). The other half of the new tokens are

   staked for downvote and left unassigned. \(Figure 3, above.\)

8. SC stakes Bob’s availability stakes as an upvote for Bob. \(This incentivizes Bob to work

   well for Alice, or he will lose his availability stakes.\)

9. Validation pool is announced to all experts to vote on. The staking process will remain

   open for a limited amount of time, set as a parameter. \(Within each expertise, the bench

   decides this expiration time. See §​9.1 Expert parameter maintenance​.\)

10. During this time, any other domain-specific sub-token holders will have the opportunity to stake their tokens as up- or downvotes, using symmetric key encryption3 to hide their

    vote from the other experts. \(Figure 4, above.\)

11. When the validation pool ends, voting parties send their decryption keys to reveal up- and

    downvotes. The winning parties will be awarded their staked amounts plus the pro-rata share of the losing party’s stakes. If Bob’s work is validated, he will be paid in tokens in proportion to the ETH staked in his name, and his pro-rata share of the losing party’s token stakes.

In summary, Semada core

1\) answers queries about the list of expertises, the list of experts within each expertise, and each expert’s availability stakes

2\) answers validation requests, taking as input an ETH fee and the address of an Ethereum post, then

a\)  distributes the ETH as reputational salaries to the bench

b\)  opens a new validation pool

c\)  collects reputation stakes from experts on the pool



## New experts

To become a ​new expert​, a public user Alice posts a comment in the forum with a pointer to a previous post in the expertise and adds a fee in her name. Following the protocol for whenever a fee is added to the platform, new tokens in the expertise tag are minted. Half the new tokens are staked for Alice; half are staked against. Experts evaluate her post by staking their reputation in the betting pool. If Alice’s comment wins, she is vested by the validation pool with reputation in the expertise linked to Alice’s pseudonymous public key identifier, and she becomes a new expert. If Alice’s comment loses, she loses all her reputation in the expertise and returns to the public.

The 50/50 stake guarantees a new expert cannot simply buy expertise, as the previous experts have complete power to decide whether the new expert has contributed positively to the platform.

## New expertises

To create a ​new expertise tag​, a public user Adam posts a new root comment in the forum and adds a fee in his name. The system then follows protocol, automatically vesting Adam with reputation in the new expertise tag. Specifically, new sem tokens are minted in the amount of the fee chosen. Half the new tokens are staked for Adam; half are staked against. Since no other experts exist to evaluate the post, the Adam’s comment wins the tie, and he is vested by the betting pool with reputation in the expertise.

Adam then has complete power to add further posts linked to this to the forum, improving the expertise tag with mission statements, protocols, evidence of expertise, and advertisement, to encourage new experts to join and eventually attract public fees for off platform expert work. Adam has complete power to accept or reject the second expert to join the expertise’s bench.

The forum will serve as a testing ground and evolutionary ecosystem for proving good practices within each expertise. In particular, to encourage public use of the expertise, smart contracting template code should be suggested by experts and continually subjected to the improving process of critical comments. Policies, evidence of experience, evidence of successful work, and advertisement for services will also be continually added and improved in the forum.


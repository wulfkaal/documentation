# DAO Life Cycle



Here we illustrate how a group may pick parameters ci and qi in the toy example of a DAO devoted to product reviews. In particular, imagine a collaboration of expert software testers.

The basic business model is that the experts create value in the beginning by reviewing software for free and posting their judgments on the blockchain with a hash of the program. The other DAO members will validate their tests using algorithmic protocols developed in the forum. Public users freely access the reviews and may trust a download if its hash matches a validated program. Later, once the public relies on the service, the DAO will attract fees from companies which want their releases validated swiftly.

The life cycle of this toy model DAO will be analyzed in 5 stages. In practice, there would be more stages which would repeat and overlap. Further, each division of a company \(each expertise\) will not experience the same stages contemporaneously with other divisions.

## Stage 1. Protocol development

The DAO first must decide how the group is organized, how power will be shared, what regulatory and legislative governance process will be used. Secondly, the DAO specifies how to perform software analysis—what logical and statistical tests are used on what types of software. Thirdly, protocols for validating another expert’s work are specified. Such protocol development is encouraged by setting parameters as follows.

1. The DAO is not attracting public fees until Stage 5, so sem tokens are minted in proportion to minimal DoS fees paid entirely by the poster. Therefore c1 is set to a very large value for these posts, to encourage protocol development.
2. The small founding group is expected to be highly collaborative so contentious debate posts move quickly to non-contentious posts, establishing precedent. Default parameters for most hard protocols should suffice when cooperation is strong, but to encourage contributions, collaboration, and consensus, the following variations may be made:

   1. The fraction of newly minted tokens staked for the post is set to c2 &gt; default = 1/2 to encourage brainstorming over policing.
   2. The fraction of newly minted tokens staked in the poster’s name is set to c3 &gt; default = 1/2 to encourage contributions over policing.
   3. The contentious debate period c9 will be short, on the order of days or weeks, with the number of validation periods c10 small.
   4. The limit to revaluation q2 &gt; def ault = 1 . This limit will be set high, so that once consensus is reached on protocols, the value of each member’s contributions can be quickly revalued to the appropriate level.
   5. The leaching value q4 is initially set to 0 so references can create new sem without punishment. Later, when small variations of the protocols for analysis or new variations on smart contracts are needed, the leaching value will be raised so that original contributions can be properly valuated.

## Stage 2: Talent Recruitment 

Once the founding members have established satisfactory sem holdings, the DAO will recruit more software evaluator experts, requesting applications to be posted to their forum for validation.  

1. The proportion c1 of sem tokens minted from the minimal DoS fees paid by the recruit will be set to determine a recruit’s initial sem holdings. c1≫default = 1 is expected to entice new experts.
2. c2 will be default.
3. c3 &lt; default = 1/2 to encourage policing.  The recruit’s application will move quickly from loosely-coupled to tightly-coupled to force consensus in a reasonable time period c9 on the order of days.

## Stage 3 Collecting Evidence of Expertise

Experts advertise their credentials and produce work-evidence posts without collecting public

fees—evaluating software for free. So they will be posting with minimal DoS fees, and c1 will again be adjusted to account for a fair valuation of the benefit to the group. c1≫default = 1 expected. Further,

1. The fraction of newly minted tokens staked for the post is set to  c2 &lt; default = 1/2 to encourage careful policing as flawed analyses are dangerous to the future of the DAO. 
2. The fraction of newly minted tokens staked in the poster’s name is set to  c3 &gt; default = 1/2 to encourage contributions since posters are not receiving fees.
3. These posts are tightly coupled and non-contentious as reviewers are following protocol developed in Stage 1. The termination period c9 will be short since validation is algorithmic.
4. The limit to revaluation q2 &gt; default = 1 is set high so the value of each expert’s contributions can be quickly revalued fairly. At this point the DAO is still not earning fees so there is less fear of attacks.

Software evaluators follow the protocols for referencing the algorithms designed in Stage 1 to fairly reward developers’ work according to their value.



## Stage 4. Attracting fees. 

Once a body of work is established, this stage requires a new effort to attract users, both general public and software companies which send fees.

  
1. The proportion c1 of sem tokens minted is set to c1 ≥ def ault = 1 to encourage experts’ focus on working hard on off-chain jobs.

2. The proportion c2 staked in favor of the post is set to c3 ≤ default = 1/2 ​to encourage policing during this crucial period when the DAO must focus on satisfying customers.

3. c3m tokens are staked in the original poster’s name. So we set c3 = default = 1/2 to balance the incentives of encouraging off-chain work and policing.

## Stage 5. Policing off-chain work

At this stage members are attracting fees from off-chain work for software companies and posting work-evidence to the forum for validation. The protocol is that a company downloads a template request for work \(RFW\) smart contract that the DAO has written and posted to their forum and chooses several parameters that the DAO has suggested, including the amount of work requested and the fee they are willing to pay. This RFW smart contract selects a random DAO member for off-chain analysis of their product. This random selection requires DAO members to have already posted availability stakes using their own smart contract, which encumbers part of their sem holdings to be engaged for off-chain work. The RFW smart contract engages Semada core, which uses a pseudo-random number generator \(with a seed which prevents stake grinding52\) to select a member weighted by their availability stakes. The randomly selected availability-stake smart contract engages with the RFW smart contract to allow the selected reviewer to post their review to the forum for validation, with the fee sent in their name to Semada, so that half of the newly minted sem tokens are staked in the reviewer’s name. The fee from the software company is distributed to the DAO in the sem-weighted salary.

1. The ratio c1 of fees to newly minted tokens is adjusted to the standard for work-evidence posts \(default c1 = 1 \).
2. The fraction of newly minted tokens staked for the post is set to c2 &lt; default = 1/2 to encourage careful policing.
3. The fraction of newly minted tokens staked in the poster’s name is  
    c3 = def ault = 1/2 . Assuming the poster follows algorithmic protocol and wins

   the validation pool, half the newly minted tokens go to the poster who does the off-chain work, and half are distributed to the rest of the DAO who police the action.

4. These posts are tightly coupled and non-contentious as reviewers are following protocol developed in Stage 1. The termination period c9 will be short since validation is algorithmic.
5. The limit to revaluation q2 is now set low \( q2≪1 \). References no longer need to revalue member’s contributions as quickly now that the platform is attracting

   steady income, so continual posts allow gradual and stable adjustments when needed. This gives the DAO added security since currency fees are now a target for attacks. Software evaluators follow the protocols for referencing the developer posts designed in Stage 1 to fairly reward the creators of the algorithms being used. The standards for choosing reference weights is set in the forum as soft protocols. Violations are algorithmically checked by members’ UI and flagged for downvoting.

6. Similarly the leaching value q4 is set to 1 so a work-evidence post can share its value with the protocol development post used, ultimately motivating continued

   development. Since work-evidence posters lose value, the soft protocol standards for referencing must be policed as described above.

Then the life cycle of the DAO will repeat as innovation research would require new protocol development to keep the organization relevant to the changing market.


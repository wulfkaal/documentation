# Sockpuppet Protocol

Background:

The basic Web of Trust \(WoT\) works as follows: Keep track of your network transactions, and ask how well the people who are part of your transactions are satisfied with the interaction. If they also have a big reputation and are satisfied with the transaction then your reputation goes up. If you get a lot of these good transactions then you have a good reputation. It's bootstrapped with early adopters who are all trustworthy. If someone behaves badly their reputation will drop.  


Here's the problem. If I use a lot of sockpuppet accounts, I can raise my reputation arbitrarily high, by behaving well for a while, then making a lot of transactions with myself and rating myself high.  


So the solution that is always offered is to control entry by identity verification. The problem with this is, if the reputation is genuinely valuable, a sockpuppet account can afford to go through whatever hoops you have in place to create false identities \(including stealing biometric data if necessary\), then increase their reputation arbitrarily, as described above.  


If the reputation is not valuable, then you won't be able to get honest users to go through the hoops required to identify themselves securely, since it's not worth it.  


So the only time WoT works is when the service is not valuable, such as PGP \(email which is essentially free\). Then it's not worth it to create sock puppet accounts, so in that case you can trust the WoT network.  


If you are trying to create an economic solution that is worth real money, where you need to be able to trust the other people in the network will behave well and follow protocol, you can't just assume their historical good behavior will prove their future behavior will also be good. Sockpuppet accounts allow us to automatedly game the system and falsely create valuable reputation, so we can leach whatever value there is out of the system.  


The voting algorithm of Semada core is designed to combat that very system, so that it is not economically feasible to game the system without adding genuinely valuable improvements, as proven with the fees that are added to the system and the fair validation pool that every fee is subject to.  


In summary, the Web of Trust is a traditional attempt to create decentralized reputation which is critically flawed and should not be used when fungible currency is at stake:

* It counts the number of transactions that are positive/honest and how much each member supports the other members  \(web of trust\) - many DLT startups use this approach
* However, sockpuppet accounts can grow their value much quicker in the web of trust by validating each other. Honest users are much slower than the sockpuppets validating each other. Hence, the system is flawed.

Here is how Semada fixes this web of trust sockpuppet flaw:

![](https://lh6.googleusercontent.com/NXNArD5yPXYGZLb450TTD4i5YA5pWhtZtJlO-LVMGzn9ll1YH_rBj55xSY-Ka9DT9syyLRy1a_ZPZdcItTn-XFMYKSCRKY6g1DqOP5gdM984D16nI5C0_cEmXwaeCYbEysTDiJ7X)

Figure 7: Figure 7 demonstrates that multiple sockpuppet accounts with 1 token each are still equal to a higher token amount of the same DAO member with only one account. In the Semada Persona Protocol, people, e.g. DAO members, can use sockpuppet accounts but they are wasting their efforts. Semada uses validation pools to make any change in rewards. All power comes from  validation pools in relation to what DAO members stake, and all fungible currency rewards are shared fairly with the group in proportion to their individual reputation. The Sockpuppet Protocol thus breaks the incentives for Sybil attacks.  



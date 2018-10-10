# Low Volatility Currency / Stable Coin

The evolving decentralized commerce necessitates stable cryptocurrencies. Yet, the emerging cryptocurrency market is afflicted with significant volatility. Unlike its centralized counterparts, the cryptocurrency market is not subject to centralized policy making via fiscal and monetary policy tools that ensure the management and stability of purchasing power of cryptocurrencies. Decentralized commerce, in turn, is less likely to evolve if the average consumer cannot rely on the enduring purchasing power and stability of cryptocurrencies over time.  

The Semada native cryptocurrency \(SEM\) is pegged to the US Dollar.  To ensure that the SEM/US Dollar exchange rate is stable at around one US Dollar, the Semada Stability Mechanism \(SSM\) provides core policy tools that help adjusts the supply of SEM in response to  SEM price movements. Similar to earlier attempts in the Basis model, the mechanism enabling price and purchase power stability in SSM involves 3 tokens: 1. SEM, 2. BONDS, and 3. SHARES. SSM uses the Semada core voting algorithm for decentralized autonomous organizations \(Stability DAO or SDAO\) to improve the Basis model in several core policy functions in a fully decentralized and autonomous way. We illustrate the mathematical limits of crash and burn scenarios of earlier attempts and contrast them with our own stability mechanism and its theoretical limits.    


**Table of Contents**  


[**1  Introduction 3**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.qzz3x6di7gl1)

[**2  Related Research 3**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.pm4d23d3htw0)

[**2.1 Critique of Robert Sams 3**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.2zu03v1tdg37)

[**2.2 Critique of Basis 4**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.i7u7w7afx77)

[**3 Semada Stability Mechanism 4**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.798onxqnlb0)

[**3.1 Stability DAO 4**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.yk01fvy6ajc6)

[**3.2 Exchange Rate Calibration 5**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.qm8yiwb87b8o)

[**3.3 Token Mechanics 5**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.6q14q08rbmpa)

[**3.3.1 SEM 5**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.ph8h9wyfqhzu)

[**3.3.2 BONDS 6**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.d6v6xabqi80q)

[**3.3.3 SHARES 6**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.950j73s2915s)

[**3.4 SEM Price Stability 6**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.mmuufmb7bclf)

[**3.4.1 Overvaluation 6**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.ybn4ue32up38)

[**3.4.2 Undervaluation 7**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.1yddhkot1u8t)

[**4 Crash-and-Burn Cycle Analysis / Model 7**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.ifghp2shrnb0)

[**5 Use Cases of a Stable Currency 8**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.9o55py1177ph)

[**6 Simulation Analyses 8**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.yajxu2bz4w3w)

[**7 Summary and Conclusion 8**](https://docs.google.com/document/d/1OlSX__to7j-EkSbwclts0pRbmJ5v60ggRyh3QowHUMI/edit#heading=h.93cwizyo70m1)****  


  
**1 Introduction**

**This paper builds on earlier research that has attempted to provide a framework for a stable cryptocurrency. We make several core improvements.**  


* **First, we introduce the existing research and provide a critique.**
* **Second, we show how Semada’s core architecture decentralized autonomous organizations helps decentralize existing attempts at stability mechanisms for cryptocurrency with governance and decentralized selection mechanisms for consumer price index selection, among other improvements.**
* **Third, we illustrate the mathematical limits of crash and burn scenarios of earlier attempts and contrast them with our own stability mechanism and its theoretical limits.**

## **2 Related Research**

* **Robert Sams, A Note on Cryptocurrency Stabilisation: Seigniorage Shares, First Version: October 24, 2014 This Version: April 28, 2015**
* **Basis Whitepaper**
* **Ferdinando M. Ametrano, Hayek Money: The Cryptocurrency Price Stability Solution \(August 19, 2014\). Located at http://ssrn.com/ abstract=2425270 or http://dx.doi.org/10. 2139/ssrn.2425270**
* **Maker DAO**
* **Tether**
* **Bitshares**
* [**https://www.reserve.org/**](https://www.reserve.org/)
* [**https://www.fragments.org**](https://www.fragments.org/about/#team)
* 
### **2.1 Critique of Robert Sams**

### **2.2 Critique of Basis**

**After review of the leading stable coin mechanisms, Semada is using the Basis paper with the majority of assumptions therein as the foundation for the SSM. Yet, several important critiques of the Basis stability design llead us to desire core improvements over the Basis paper:**

* **We use SDAO to fully decentralize the oracle function in Basis**
* **Rational self interested actors as SHARE owners can create a significant risk to the success of the Basis stable coin.**
  * **Basic assumptions for this scenario analysis**
    * **The calibration of SEM, BONDS and SHARES as described below results in a stable SEM**
    * **SEM demand grows linear over time with more consumers adopting SEM functionality and use on the Semada platform**
  * **If these assumptions hold true, rational SHARE owners will hoard SEM and not release them to the general public because as long as all rationally acting SHARE owners do not sell SEM to the public the Semada platform, the SSM, and the SDAO will have to continue to authorize the minting of new SEM to keep the currency stable, satisfy consumer demand, and guarantee the functioning of Semada platform.**
  * **This creates several issues for the future of SEM**
    * **Without sufficient availability of SEM for the public, Semada platform cannot function effectively as all functions depend on the availability of SEM**
    * **SHARE owners who are hoarding create artificial inflation for SEM**
  * **SSM addresses these issues by:**
    * **by loaning out the newly minted SEM to those consumers who will use it immediately--those that are demanding it and driving the price up.**
    * **SSM guarantees the availability of SEM to the public through a natural market for SEM loans.**

## **3 Semada Stability Mechanism**

### **3.1 Stability DAO**

**Semada’s Stability DAO \(SDAO\) creates a core improvement over existing stability mechanism for cryptocurrencies. SDAOs is needed for multiple oracle functions in the stability mechanism and enables an unprecedented fully decentralized stability model. Some of its core improvements include:**

* **Fully decentralized policy decision making**
* **Full transparency of policy decision making**
* **Determination of the SEM / US Dollar exchange rate**
* **SEM monetary and fiscal policy decisions**
* **BOND token pricing and issuance decision \[no. Market decides pricing via auction.\]**
* **SHARE token pricing and issuance decision \[I don’t think so. SHARE tokens will probably all be gone to investors when SDAO starts.\]**
* **Determine BOND expiration date \(e.g. 5 years or less\) for each BOND issuance \[yes, but I suggest no expiration date; they should all be paid off.\]**
* **Select a Consumer Price Index \(CPI\) for the peg \(removing the US Dollar peg\)**
* **SDAO determines artificial bond token price floor to ensure SDAO does not borrow excessively in attempt to limit SEM supply**

**Benefits:**

* **Maintain a fully decentralized policy mechanism**
* **Full transparency of policy decisions**
* **No need to remove human decision making via automation to retain benefits of decentralization**
* **Fully transparent policy making that allows the public to anticipate when the SDAO will mint new tokens. SEM may autocorrect to equilibrium exchange rate of  1 US Dollar**

**Risks:**

* **Inability to react to market movements in real time \(mitigation possible over time via decision making automation - yet automation of decision making would rely on incomplete and historical data and is risky given changing market environments and inability to apply decision precedent in historical market environment to the future and future states\) - Monte Carlo simulations cannot fix this issue as they rely on historical data**
* **Robustness of SDAO decision making - can the SDAO truly anticipate when policy reactions are needed?**
* **Delineation of automation of policy decisions via algorithm vs. SDAO intervention \(this should materialize over time\)**

### **3.2 Exchange Rate Calibration**

**Existing cryptocurrency exchanges provide data feeds on exchange rates of cryptocurrencies to the US Dollar. Yet, cryptocurrency exchanges that provides sufficient liquidity, such as Coinbase, Binance, Kraken, Poloniex, and Everex, among others, are centralized. SSM provides a decentralized solution for the determination of the SEM/US Dollar exchange rate via the SDAO. This decentralized exchange rate calibration has several benefits in comparison with existing solutions:**

* 
### **3.3 Token Mechanics**

**SSM accomplishes the calibration of pricing mechanism for SEM through the triangulation of 3 tokens, 1. SEM, 2. BONDS, and 3. SHARES.**

#### **3.3.1 SEM**

* **SEM tokens are the native currency of the Semada platform that is the subject of the stability mechanism.**
  * **SEM are pegged to the US Dollar**
  * **SEM are fully fungible and will be listed on an exchange to provide investors with liquidity**
  * **The SEM token supply is the subject of the stability mechanism**

#### **3.3.2 BONDS**

* **BOND tokends are Semada platform tokens that are minted by the Semada platform and issued at a discount if and when the desired exchange rate of SEM to US dollar is below the desired exchange rate of 1 SEM = 1 US Dollar.**
  * **BONDS are auctioned off at a given market price at the time of the auction**
  * **BONDS are free floating and not pegged to anything**
  * **BOND owners speculate on the price improvement of SEM over time and profit off the spread between bond issuance price and SEM price upon conversion of BONDS to SEM.**
  * **BONDS are subject to the pricing mechanism by the SDAO**
  * **BONDS tokens give the token holers the right to convert back to SEM if the SEM price reaches the desired exchange rate of SEM = 1 US Dollar.**
  * **BOND conversion into SEM / redemption is possible only when:**
    * **All BONDS from prior BOND issuance have been converted/redeemed or expired**
    * **Current BONDS have not expired \(and qualify for redemption\)**
    * **SDAO decided the expansion of the SEM supply is warranted**
    * **Semada platform started minting new SEM**
    * 

#### **3.3.3 SHARES**

* **SHARES are native genesis Semada platform tokens that are issued in limited and final supply of  \[\_\_\#\_\_\] tokens.**
  * **SHARES are not pegged to anything**
  * **SHARES have secondary priority for SEM token payouts after all BONDS from any issuance have been redeemed or expired.**
  * **SHARE token holders may not receive any SEM payouts if the SDAO in the interim e.g. after a given BOND issuances, authorizes and initiates another BOND issuance/auction**   
  * **SHARE token holders receive SEM payouts as dividends if and when all BONDS were exchanged for SEM and the SEM market price is still below the intended US Dollar exchange rate of $1.**
  * **SHARE tokens are subject to the pricing mechanism determined by the SDAO**

### **3.4 SEM Price Stability**

**SEM price stability is accomplished through the interplay of SEM, BONDS and SHAREs**  

#### **3.4.1 Overvaluation**

* **If SEM is valued above $1, then mint via SDAO SEM to lower demand by increasing supply, resulting in price correction back to $1.**
* **The following procedures apply to the overvaluation correction:**
  * **SDAO decides that overvaluation merits minting SEM**
  * **SDAO tallies any existing and outstanding BONDS and SHARES \(automation over time after SDAO triggers minting\)**  
  * **Newly minted SEM are distributed to 1. BOND token holders, and 2. SHARE token holders in order of priority**
    * **All existing BOND holders are paid first, unless their BOND expired, in First in First out Order until no BOND holders remain**
    * **After the last existing BOND holder was paid in SEM, the platform automatically allocates any additional newly minted SEM to the SHARE holders pro rata, as dividends**

#### **3.4.2 Undervaluation**

* **If SEM is valued below $1, then burn SEM to increase demand by cutting supply.**
* **The following procedures apply to the undervaluation correction:**
  * **SDAO decides that a BOND auction is warranted \(automation over time after SDAO triggers BOND auction\)**
  * **SDAO determines artificial bond token price floor to ensure SDAO does not borrow excessively in attempt to limit SEM supply**
  * **Market demand in auction determines BOND price**  
* **Open issues: \*\*\***
  * **If Semada does not have sufficient liquidity reserves to burn SEM out of the initial supply minted, Semada would have to buy back SEM on the open market ? \*\*\* If so, how will the buy-backs be funded? \*\*\***
    * **Burning of sem results in selling bonds at 70/100 \(example\) and convert bond into SEM if SEM market price reaches $1.**
  * **Alternatively, if BOND tokens can only be purchased with SEM tokens at a 70/100 discount, ceteri paribus, then BOND tokens sales would take SEM tokens out of circulation \(just like a burn of SEM tokens\) for the duration of market recovery in SEM price \( e.g. until 70 price returned to 100\)**
    * **Market signal of BOND purchase with SEM not as strong as burn\*\*\***
* **SHARES get paid dividends in SEM after all the BONDS were converted into SEM and ONLY IF the SEM exchange rate remains below 1 US Dollar.**
  * **Shares get paid newly minted SEM as dividends as long as it takes to bring SEM market back to $1 exchange rate to US Dollar.**  

## **4 Crash-and-Burn Cycle Analysis / Model**

* **Create mathematical model to assess the boundaries of the crash and burn cycles that are theoretically possible in the Basis model**
* **Contrast crash and burn cycles that are theoretically possible in SSM - if different? \*\*\***

## **5 Use Cases of a Stable Currency**

 **Use cases of stable currency:**

1. **Provide stability for cryptocurrency market as safe-harbor for cryptocurrency investors**
2. **A native network digital currency that is stable and can be used for decentralized commerce**
3. **A currency as a replacement for paper fiat currency for countries \(e.g. peg. Countries can issue digital currencies by pegging it to SEM\)**
   1. **Target market: Governments looking to setup a digital currency**
   2. **Sell Semada stability mechanism software to different countries**
   3. **Enabling and full integration of currency, creating currency pegs**
   4. **Create other currencies on Semada**

## **6 Simulation Analyses**

**This section contains numerical analyses for the procedure described in our mathematical model. We also conduct a sensitivity analysis for several input parameters. In particular, we study the impact of the parameter specification of the \[\*\*\*\].**  


**EXPLAIN AND SHOW WITH GRAPHICS AND NUMERICAL EXAMPLE**  


## **7 Summary and Conclusion**

**Open issues:**  


**Initial Peg SEM/US Dollar - later CPI peg through the SDAO decision**

**Calculation / simulation as to when it is stable -**

**SHARE holders have money SEM but they cannot control the SEM that come to the SHARES - Semada puts that SEM on the Market for ETH BTC etc. in order to liquidate it.**

**Hoarding only an issue until the network gets large enough**

**We should be open and say that we control the SHARES - the SHARE holders hold the**

**Semada takes a fee for the service of selling the SEM that were allocated to the SHARE holders to the market and selling it.**

**We probably need to give the SHARE holders assurances that we will cover the exchange rate risk. Semada liquidity treasury team has to guarantee to SHARE holders the full maket price.**

**Solution: 50% of SHARES to investors**

**50% of SHARES to SRI**

**Lending market for SEM via the SHARE - as second benefit for SHARE ownership**

**MInt SEM goes to SHARE and then buy it on the market Binance etc. to buy**

**SHARE holders cannot keep SEM and have to sell it to the market - but exchange risk to the SHARE holders**

**Black Swan event if hoarding SEM or economy collapses - then actual value of the SEM is not what the peg is. REsulting in crisis of confidence. You cannot hold the peg then, so SDAO should have power to judge whether the system is in that state and repeg.**  


**Distribution mechanism of SEM -**  


**SDAO functioning:**

* **Should be in charge of the SEM that the SHARE holders collect - always \[no, not always, just in case of the unlikely scenario that someone corners the share market and holds SEM in order to drive up price \]**
* **How does that SEM get to the market**
* **SHARE holders get only cash not SEM \[not usually\]**
* **SHARE holders own SHARES but do not control them with regards to the SEM revenue received \[not usually\]**
* **Income for SHARE owners as fair price for**
* **SDAO in conjunction with the Semada Treasury team guarantees conversion risk**
* **KYC / AML issue - account that settles USD - settle in crypto ?**
* **Force people to convert into BTC that then stabilizes BTC ?**
* **Liquidity for SHARE holders - Semada sells the SEM on the market for BTC and give the BTC to SHARE holders - legal and tax implications -**
  * **We would be creating an exchange**
  * **Partnership with an existing exchange**
  * **Reconcile with your SHARE holders**
* **Semada is centralized until it scales**
* **Alternative mechanism to remove the holding process for SHARE**
  * **Exchange solution ?**
  * **SHARE holders to dump their SEM currency - take advantage of arbitrage on different exchanges ?**
  * **50% only sells to market**
* **3 Proposals as to how to do with the issue of wealth centralization in SHARE holders \(hoarding\)**
* **1. Proposal against wealth centralization:**
  * **When SEM minted not given to SHARE holders but open to people to get SEM for BTC**
    * **Smart contract determines when SEM minted**
    * **SEM waiting for exchanges to buy them with BTC**
    * **Anybody who buys via smart contracts the SEM via BTC**
    * **Then BTC send to SHARE owners**
    * **SDAO determines the exchange rate before the minting**
      * **Smart contract uses BTC address to send the SEM**
      * **Smart contract can use an atomic SWAP as long as it has the same hashing algo**
      * **Why not use same exchange**
      * **Problem: We are using a non-native currency to settle in the network - not sure if this can work from an implementation network perspective**
      * **Simulate BTC - as a financial product ?**
* **2. Proposal against wealth centralization:**
  * **Economic cycle and development phases to address the SEM hoarding by SHARE owners \(may not be a real problem\)**
  * **Phase 1: SHARE get SEM, if no wealth centralization stay in phase 1 without additional policy changes. If wealth centralization detected, then trigger policy changes e.g. moving to Phase 2.**
  * **Phase 2: SHARE owners loan SEM to public as needed. If no wealth centralization stay in phase 2 without additional policy changes. If wealth centralization detected, then trigger policy changes e.g. moving to Phase 3.**
  * **Phase 3: SHARE surrender SEM to Semada in exchange for payouts**
* **3. Proposal against wealth centralization \(SHARE token holder hoarding of SEM\):**
  * **Token design to Stimulate Valuable Economic Activity on the Network:**
    * **Core improvement over Basis and any other stability token that does not serve a network:**
      * **Use stable SEM currency to stimulate Stimulate Valuable Economic Activity on the Network**
      * **BTC vs. ETH - ETH is actually used**
    * **Determine metrics for allocating SEM between economically valuable activity on the network \(e.g. SPOS DAO, among other valuable activity on Semada\) and allocation to SHARE token holders**
      * **This may avoid wealth centralization, e.g. hoarding by SHARE owners altogether**
      * **The market should correct this attack - it should be a remote event.**
      * **ONLY use this as a checks and balance on the power of the SHARE holders in a black swan event:**
        * **SPOS DAO is the only DAO that gets the SEM salary bump if SDAO detects \(using computer algorithms\) inflation/ aggregate hoarding by SHARE holders results in minting more SEM. Wealth centralization detection result in minting SEM.**
    * **Problem in this approach?**
      * **Negative signal if algo gets triggered?**
      * **Moving away from incentives to increase reputation? E.g. is an SPOS holder who gets a payout bump in SEM via the wealth centralization avoidance mechanism/algo disincentivize to increase SPOS reputation ? Probably not because SPOS holders don’t build their SPOS reputation in anticipation of the SEM bump from the the wealth centralization avoidance mechanism/algo**
  * **We would need a model to understand where the wealth centralization avoidance mechanism/algo should kick in and at what proportion/level**

**What if the market does not buy the BONDS? I.e. no speculators want to take the risk for a SEM discount**  
  


**Control shareholder share until network is**  


**Listing Decision:**

* **List SHARE ownership for INVESTORS**
  * **List as securities token in secondary market on T-zero**
  * 
* **List SEM - after picking use case**
  * **Semada currency technology -**


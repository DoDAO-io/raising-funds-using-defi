## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Chicken bonds
 
 
---

##### What is the main purpose of chicken bonds?  

- [ ]  To make large profits for the protocol’s team
- [ ]  To create new tokens
- [ ]  To increase the price premium of stablecoins
- [x]  To bootstrap liquidity of protocol
  
Hint: NoHint
         
Explanation: To deepen the liquidity reserves a protocol.

Sub Topics: No Sub-Topics
 

---

##### What makes chicken bonds stand out from other bonding / staking mechanisms?  

- [ ]  Bonds without a maturity period, users can withdraw their deposited funds anytime given they have not already chickened-in
- [ ]  Wrapping bonds in NFTs which can be sold
- [ ]  Enables the protocol to bootstrap liquidity without funds from external entities
- [x]  All of these
  
Hint: NoHint
         
Explanation: Chicken bonds gives flexibility to the users who have bonded  to be able to withdraw their funds at any moment without losing any principal amount and also to the protocols to own their liquidity.

Sub Topics: No Sub-Topics
 

---

##### What do the terms chicken-in and chicken-out mean?  

- [x]  Chicken-in means to forsake user’s possession of the deposited underlying token in return for the accrued bToken
- [x]  Chicken-out means to quit the bond and take back the user’s deposited underlying tokens
- [ ]  Chicken-in means to quit the bond and take back the user’s deposited underlying tokens
- [ ]  Chicken-out means to forsake user’s possession of the deposited underlying token in return for the accrued bToken
  
Hint: NoHint
         
Explanation: Chicken-in means to forsake user’s possession of the deposited underlying token in return for the accrued bToken and Chicken-out means to quit the bond and take back the user’s deposited underlying tokens

Sub Topics: No Sub-Topics
 

---

##### How can users earn money using the chicken-bonds?  

- [ ]  The users can sell the NFTs of the bond at NFT marketplaces, especially if the NFT generated is a rare one
- [ ]  The users can become LPs by investing bTokens in Liquidity pools
- [ ]  The users can redeem the accrued bTokens for the underlying tokens and make a profit if the accrued bTokens have reached breakeven with the deposited underlying tokens
- [x]  All of these
  
Hint: NoHint
         
Explanation: Users can earn money by redeeming the accrued bTokens for the underlying tokens and make a profit if the accrued bTokens have reached breakeven with the deposited underlying tokens, by investing bTokens in Liquidity pools, and by selling the NFTs of the bond at NFT marketplaces.

Sub Topics: No Sub-Topics
 

---

##### Which of these are the buckets used in chicken bonds?  

- [x]  Reserve bucket
- [x]  Pending bucket
- [x]  Permanent bucket
- [ ]  Chicken-in bucket
  
Hint: NoHint
         
Explanation: The buckets used in chicken bonds (b.protocol) to segregate user deposited funds are Reserve, Pending and Permanent buckets.

Sub Topics: No Sub-Topics
 

---

##### Which of the following statements are true regarding buckets in chicken-bonds?  

- [x]  When the user deposits money in chicken-bonds, it first goes to the Pending bucket
- [ ]  When the user deposits money in chicken-bonds, it goes to the Reserve bucket first
- [ ]  When the user deposits money in chicken-bonds, it goes to the Permanent bucket                   first
- [ ]  When the user performs a chicken-in, the chickened funds all go to the Permanent bucket
  
Hint: NoHint
         
Explanation: The assets that the user uses to bond are initially stored in the pending bucket.
If the user then decides to chicken-in, their funds are sent to the Reserve (according to the bTokens generated, to keep the backing ratio constant)  and                 Pending buckets (The tokens left over after depositing funds in the Reserve bucket). Note: this is not the order of the flow, but the logic of it.


Sub Topics: No Sub-Topics
 

---

##### Which of these factors make sure that the backing ratio ( tokens in reserve bucket / boosted token supply) always increases?  

- [ ]  The percentage increase in total number of bTokens is always kept constantly proportioned to the amount of underlying tokens in the Reserve bucket
- [ ]  The percentage increase in total number of bTokens is always kept constantly proportioned to the amount of underlying tokens in the Pending bucket
- [ ]  The Reserve bucket keeps accumulating yield from all the three buckets because of which the backing ratio will keep increasing between subsequent chicken-in events.
- [x]  Both A and C are true
  
Hint: NoHint
         
Explanation: After every chicken-in event, an amount of underlying tokens is sent to the reserve bucket such that the current backing ratio remains constant, i.e the percentage of increase in underlying tokens in the Reserve bucket will always be constantly proportioned to the percentage increase in the total number of bTokens. And, Reserve bucket accumulates yield from all three buckets, constantly increasing the backing ratio.

Sub Topics: No Sub-Topics
 

---

##### bTokens can be redeemed for a pro-rata ration of the Reserve bucket.  

- [x]  “True”
- [ ]  “False”
  
Hint: NoHint
         
Explanation: True, if a user holds x% of the total bTokens supply, they can redeem it for x% of the total amount of underlying tokens in the Reserve bucket. (Note that, bTokens could be acquired by chickening-in bonded funds or by buying it from a DEX)

Sub Topics: No Sub-Topics
 

---

##### Which of these could be viewed as an advantage of using chicken-bonds (from the protocols perspective)  

- [x]  Can provide a sustainable incentivization to users for long term participation
- [ ]  Can help to hold a hard peg on the underlying assets
- [x]  The protocol can bootstrap liquidity by simply letting users use their protocol and not by external funding
- [ ]  Chickens bonds are unsustainable in the long term because it requires heavy funding
  
Hint: NoHint
         
Explanation: It ensures that the protocol can incentivize users for long term participation since long term participation of users does not mean that the protocol needs to bring extra capital (unlike in staking). Can help to hold a soft peg on the underlying token, if needed.

Sub Topics: No Sub-Topics
 

---

##### Which of these is a possible drawback of chicken-bonds and bTokens?  

- [ ]  The user can sometimes be locked from chickening-out
- [x]  The breakeven time for a bond could be too long for a user to make it profitable
- [x]  Buying bTokens at a premium from a DEX might not be useful if the APY offered for being an LP is not profitable.
- [ ]  bTokens might not yield more than the underlying tokens
  
Hint: NoHint
         
Explanation: The breakeven (the time taken for the accrued bToken to cross the value of deposited underlying token) time could be too long to make the bonding profitable. In these times, user might want to buy bToken from a DEX and become an LP, but that could also be not profitable since bTokens trade at a premium above their price and the LP APY might not be enough to compensate for the premium.

Sub Topics: No Sub-Topics
 

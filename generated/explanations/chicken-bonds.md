## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Chicken bonds
 
 **Introduction**        
### Introduction

Chicken bonds was one of the most successful implementations in the DeFi space of 2022, let us understand what it is and why it is used. 

Chicken bond is a novel bonding mechanism, which allows protocols to deepen the protocol owned liquidity of their own token. In chicken bonds, users bond an amount of the protocol tokens in turn for virtually accruing newly issued boosted tokens (bTokens) which have a higher return than the yield on the underlying token.  After some time has passed, the user can decide whether to mint the bTokens which have accrued virtually and give up their possession of the underlying tokens (Chicken-in) or to cancel the bond and get back their principal amount of the underlying token (Chicken-out). Different stages of the bond are expressed via artwork as NFTs, these NFTs can be transferred and point to the bond, meaning whoever owns the NFT is in possession of the bond. The longer a bond has been going on for, the rarer the NFT it is associated with.  The bTokens can either be redeemed for the underlying tokens from the protocol, or be swapped in a DEX depending on whichever is more profitable to the user. Moreover, the bTokens can be bought in DEXs as a form of investment if the user believes in the long term appreciation of its value. 

Now that we have briefly introduced what chicken bonds are, let us dive a little deeper and see how they work behind the scenes and some of its advantages.
 
 **Learnings**        
### Learnings

It is understood that the user bonds the protocol tokens in return for a virtual accrual of bTokens which the user can choose to claim (Chicken-in) or not (Chicken-out). But the question of how the bTokens provide more yield than the underlying tokens and how it is feasible for the protocol arises. To answer that, we need to understand where the bonded underlying tokens go. But first let us have a brief overview of the bonding itself.

Users can benefit from the system by,
* **Bonding:** The user can make a profit by bonding, achieving breakeven and then redeeming the bTokens

* **Investing:** Buy the bTokens on the market as a long-term investment with amplified returns and limited downside risks.
* **Sell the bond:** Sell the chicken-bond NFTs in NFT market places.



At any point in time, the holder of the bond can decide to:
* **Claim bond (Chicken In):** claim and mint the accrued balance of bTokens in exchange for the deposited tokens.
* **Cancel bond (Chicken Out):** retrieve the deposited tokens (principal) forgoing the accrued balance of bTokens.
* **Users can sell their bonds:** Represented as NFTs on the secondary market like OpenSea. This especially makes sense for bonds that have accrued a significant amount of bTokens without breaking even yet.
Now that we have that clear,  let us see where the bonded tokens go and how it aids in the bTokens achieving a boosted yield.
**Buckets**

Buckets are reserves of the underlying token. There are three “buckets” of tokens where the bonded tokens are held. Think of these as an internal segregation of assets by the protocol to have better clarity over how much assets they hold and make use of in different aspects of the chicken bond. 

These are Pending, Reserve and Permanent buckets. The protocol generates yield on the tokens from all three buckets and this yield from all the three buckets is funneled into the Reserve bucket and bTokens can be redeemed for a pro-rata ratio of the Reserve bucket.

**Flow**

First, when a user bonds their tokens, the tokens are sent to the Pending bucket. Then, depending on whether the user chickens in, the “chickened-in” funds are sent to the other two buckets, Reserve and Permanent.

The tokens in the Reserve bucket are directly responsible for the backing of the generated bTokens, while the tokens in the Permanent bucket are permanently owned by the system and are used to generate yield to be funneled into the Reserve bucket. 

**Boosted yield**

**Backing ratio never decreases**

Whenever somebody Chickens In, the protocol expands the bToken supply in the same proportion as it increases the Reserve Bucket backing them. Let us see how.  The protocol makes sure that the backing ratio, given by ``tokens in reserve bucket / boosted token supply`` never decreases. This means that whenever there is a chicken-in event and bTokens are minted, the amount of underlying tokens sent to the reserve will be such that the backing ratio never decreases (or remains the same as it was before the chicken-in event). 

This is done by levying a maximum cap (as we saw on the graph) on the amount of bTokens generated according to the current backing rate. The cap is defined as ``boosted_token_supply/reserve_bucket ``. 

To better understand, let us consider an example  For instance, let’s assume a user bonds 120 TKN, and the current backing ratio is 1.5. Therefore the cap for that bond would be 80 bTKN (= 120 / 1.5). After some time and reaching **80%** of the cap the user claims the bond. So the system mints 64 bTKN for the user, and the bonded amount is split in 96 TKN **(80%)** which go to the Reserve Bucket, and 24 TKN (the remaining 20%) which are deposited in the Permanent bucket.

**Boosted yield and rising price floor**

On top of the yield token always being backed at a set minimum ratio per each chicken-in event, the Reserve bucket is constantly accruing yield from the other two buckets which means that the backing ratio keeps increasing as time passes. For example, say at some time T, we had a backing ratio 1.5, at some time T+X we would have a higher backing ratio, say 2. Because the backing ratio never decreases per chicken-in event and on top of that, the amount of underlying tokens in the Reserve bucket keeps increasing owing to yield from the tokens in the other two buckets. 

Remember, bTokens can be redeemed for a pro-rata ratio of the Reserve bucket. Since the number of underlying tokens in the Reserve bucket increases faster than the total number of bTokens according to the above logic, a scenario where the price floor for the bTokens keeps increasing is created (Meaning the amount of underlying tokens redeemable for the given amount of bTokens keeps increasing, theoretically). 

**Summary and the flywheel effect**

To sum up, Given that the yield from all three buckets is sent to the Reserve Bucket, the backing ratio (price floor) will grow faster than the value of a simple portfolio of the underlying token. By pricing in the amplified growth, the bTokens should trade at a premium against their price floor, driving a flywheel: the more people bond, the more yield is retained for the bToken holders. A higher yield in turn increases the price premium, making bonding more attractive through a higher APR.

To ensure that bonding remains attractive when the premium drops, the protocol may automatically adjust the accrual rate (steepness of the accrual curve) using a controller targeting an average Chicken In time or bond age.
 
 **Advantages**        
### The advantages

Contrasting chicken bonds with another way which protocols use to deepen liquidity of their token, staking. We have seen that in staking, protocols initially offer a very high APR to attract users to deposit tokens in their reserves and thus deepen their Protocol Owned Liquidity which can help the protocol in gaining stability for their token, and credibility in the market. But these high APRs are often unsustainable and as soon as the protocol starts offering a more practical APR on staking, the users start pulling out their funds since they no longer find this to be a profitable investment. In this system we see that the protocol cannot reward users for their prolonged participation, as the APR is likely to decrease in the long run. 
On the other hand, chicken bonds help protocols deepen their liquidity by providing a novel bonding mechanism which rewards users for their long term participation while simultaneously deepening their Protocol Owned Liquidity. Ofcourse, on the user side of things there is always the issue of volatility of the bToken or the underlying token in DEXs which could mean that user incurs a loss but in theory, the user can yield more with the bToken than they would with the underlying token which is an attractive offer for the users holding the underlying token, who are the target users for this mechanism. 
 
Helps deepen the liquidity of the protocol, and to hold a soft peg. 
The bond has no maturity, meaning the user can choose to reap the benefits or quit if they do not find it to be profitable at anytime, which is often not possible in staking. This makes chicken bonds more attractive to users.
The user can obtain dynamic NFTs whose rarity can vary depending on the time that has passed since chickening in, etc. These NFTs are proof of ownership of the bonds, meaning that the bonds can be sold and bought in markets, opening new investment opportunities.
Other options of generating liquidity often involve recurring expenses from the protocol, which is unsustainable unless there is a lot of funding for the protocol. But in the case of chicken bonds, all the protocol needs to capture liquidity is time, and ofcourse users to bond, the users will start using chicken bonds when they realize that it is worthwhile.

An example of the advantage of bTokens with the use of bLUSD. Say LUSD is trading at a price premium to its $1 peg, as long as LUSD is trading above its peg, users will mint LUSD and try to take advantage of arbitrage. With bLUSD, users can get compounded yield on LUSD which makes the arbitrage option more attractive. This way, as long as there is a price premium for LUSD, users will be more incentivized to invest it in chicken bonds and reap more benefits. While simultaneously, the LUSD liquidity will be deepened, making it stabler and helping to reduce the price premium, which is what is expected of a stablecoin (to trade at peg value).
 
 **Drawbacks**        
### Drawbacks using LUSD/bLUSD as an example

Like with all protocols, the b.protocol (chicken-bonds) also has its own downsides. Let us look at a few of them with the help of Liquity as an example.

Sometimes, it could be more profitable to chicken out and simply buy bLUSD in an exchange than to accrue it from being bonded. Also, the idea of rebonding (redeeming bToken from a previous bond to bond again with a larger amount of underlying token) can sometimes prove to be too time taking and providing very little yield in the end whereas the user can just buy bLUSD and become an LP for a better yield (a user would rebond only when the bLUSD value has achieved breakeven with the LUSD invested, which can take a long time sometimes). Though as people chicken out to buy bLUSD, the rebond time to make a profitable chicken-in decreases, but the user can chicken out and not buy bLUSD at all, users might face loss in such a scenario.


bLUSD is often trading at a premium, if user buys bLUSD to become LP in a curve pool, it is very likely that the user will not be able to cover the premium that they paid using the APY being offered by being an LP. Also, it is interesting to note that as users chicken-out, the APY for bLUSD supply decreases. In the first scenario, the only other option for the user to make any progress with bLUSD being buying it in an exchange and becoming LP is again not solid, since the APY for the bLUSD supply will decrease and the bLUSD premium will be too much for the reducing APY to cover. In other words, if the rebonding proves to be not profitable, or time taking, the user might want to become bLUSD LP, but that option is also not great since the bLUSD price and the APY it earns are not at par with each other (you would want more APY than the bLUSD premium price).
 
 
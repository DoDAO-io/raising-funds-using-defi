## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Intoduction
 
 **Crowdfunding Issues **        
## Traditional Fundraising Situations
Traditional methods of fundraising can be quite limiting and outdated, often not taking into consideration new techniques that could make the project more appealing to not just venture capitalists, but to the community or customers as well. Some limitations of existing fundraising methods include:

### Problems faced by Founders
- It is easier for projects that speak VC-friendly language to raise funds, limiting access for first-time creators or founders.
- Often requiring a lot of upfront work with no guarantee of success, the process can be time-consuming and frustrating
- In most cases, founders start with a vision and mission, but due to the financial goals involved, the focus is completely on maximizing profits, with little attention given to the company's impact on society.

### Problems faced by Investors
- Price is set by the founders or VCs, without any price discovery.
- Before the product market fit is found (startup profits significantly), it is difficult to determine a price.
- VCs have to guess without knowing how the product will be perceived.
- Many investors shy away from venture capital firms because of locking cycles of 5-10 years.

### Other Pressing Issues
- A majority of investment opportunities are only available to accredited investors, i.e. people earning more than $200,000 per year.
- As companies only go public after growth has normalized, public markets aren't rewarding any more
- Most startup companies spend far more money to acquire a customer than they will ever gain from them since there is minimal transparency in the process.
- Often, your community is your product. Current business models don't allow community members to share in the gains and risks of their projects.


## DeFi Fundraising
In DeFi projects, one or more tokens can be issued and then sold by the project using some of the fundraising primitives that have been developed in the ecosystem.  One thing to note is that many of the projects in Crypto might not adhere to security laws (selling of the shares/stocks in open market) and it is very important to do your proper research before you decide to use one of the DeFi primitives for fundraising. The most common DeFi primitives for fundraising currently used are:
1. **Bonding Curves** - Bootstrapping funds with earlier investors being rewarded more lucrative than those who join the project later on.
2. **Liquidity Mining/Yield Farming** - Offering native tokens to investors in exchange for providing liquidity to the protocol which can be used for trading, lending, or borrowing. This structure allows investors to have nearly full control over the funds and they can choose to exit the position when desired.
3. **Staking** - Staking allows investors to deposit their funds with a protocol and earn interest on them. In the event of an unexpected loss of funds, some money may be deducted from the deposited funds. 
4. **DeFi Bonds** - DeFi bonds are an innovative mechanism that allows investors to purchase tokens at a discount. Investors purchase the bonds and then get access to the tokens once the bond matures.
5. **Quadratic Funding** - In this crowdfunding method, money from a central matching pool is allocated based on which projects are more democratically supported as opposed to those into which more capital goes.
6. **Liquidity Bootstrapping Pools** - 
7. **Batch Auctions** -

We will cover each of these funding methods in the following sections. 

## References
- https://medium.com/giveth/the-commons-stack-scaling-the-commons-to-re-prioritize-people-and-the-planet-fdc076aec4eb
- https://medium.com/giveth/blockchain-economies-and-the-commons-cdb67dd1a163 
 **Bondig Curves**        
### What is a Bonding Curve?

The Bonding Curves Offerings (BCO) provides a way for projects to efficiently, fairly, and reliably distribute tokens to project adopters in a transparent way. 

A bonding curve is a mathematical curve that defines the relationship between price and token supply. In other words, it's a way to visualize how the price of a token changes as more tokens are minted. Here's an example of a bonding curve, where `currentPrice = tokenSupply²`:


<img style="max-height:300px" src="https://raw.githubusercontent.com/DoDAO-io/raising-funds-using-defi/main/images/simple_bonding_curve.png" />

`Source: https://yos.io/2018/11/10/bonding-curves/`

The Bonding Curve explains how the price of a token is determined by the number of tokens that have already been minted. In the case of an exponential curve, such as the one shown in the example, the growth rate will speed up as the number of tokens minted increases.

When someone buys a token, each successive buyer will need to pay a slightly higher price per token, which could generate profits for the earliest investors. As more people learn about the project and buying continues, the value of each token will go up slowly along the bonding curve. As tokens have the lowest price at the lowest part of the curve, there is a price advantage for early adopters. Early buyers have a considerable upside potential when compared with later entrants to market, as prices are lowest when supply is low as well.

Early buyers of tokens have a considerable upside potential when compared with later entrants to market, as prices are lowest when supply is low. As tokens have the lowest price at the lowest part of the curve, early adopters can benefit from a price advantage. By getting in early, buyers can take advantage of the potential for growth as prices increase as more people enter the market.

The most significant advantage that Bonding Curves have over traditional asset pricing methods is the fact that the pricing of assets is transparent, set in stone(on-chain), and unchanging at all points. The market is able to reach a collective agreement through well-defined rules, without needing outside intervention. Because the cost per token is decided by the curve/formula, every person involved knows how much each token will cost ahead of time. This allows for a honest and just market where everyone knows the score.

### Buying/Minting tokens from bonding curve:
- A bonding curve smart contract is created that allows users to buy/mint a new token (eg. Bonding Curve Token, ABC) with by supplying a currency for example USDC.
- The price of ABC is algorithmically calculated in relation to its current circulating supply and shown in its reserve currency, USDC.
- By providing USDC to the contract, the user can buy the new ABC token through a smart contract. 
- After the user completes their purchase, the price of the token will move along the bonding curve in relation to the amount of supply the user has just minted (likely moving the price up for future buyers)
- A ABC holder can choose to burn or sell their token back to the curve at any time. If the price of the token goes up after they purchase it, they will likely sell it at a profit (minus gas and fees). They will receive the bonded USDC back from the smart contract after their sell is approved.


### Key benefits of bonding curves:
- Limitless Supply - Normally there is no limit to the number of tokens that can be minted.
- Deterministic Price Calculation - The price of the tokens increases and decreases according to the number of tokens minted.
- Continuous Price - The price of token n is less than token n+1 and more than token n-1.
- Immediate Liquidity - Tokens can be bought or sold instantaneously at any time.

### Limitations
* Basic forms of bonding curves don't keep a minimal reserve that might be needed to bootstrap the project.
* Users can buy or sell the tokens to the bonding curve, but minting of new tokens based on time schedule is not possible. This could be an issue for new projects that need to compensate for an initial burn rate.

### Augmented Bonding Curves
The most basic form of a bonding curve is "x = y." By adding more variables or constraints to the formula, you can make the bonding curve more suitable to the needs of your project. The Augmented Bonding Curve, explained below, is one such example of how bonding curves can be extended.

The Augmented Bonding Curve design can be conceptualized as a typical bonding curve with the addition of a funding pool, a token lock-up/vesting mechanism, and inter-system feedback loops. The system is launched in two stages: the Hatch Phase and the Open Phase.

<img style="max-height:600px" src="https://raw.githubusercontent.com/DoDAO-io/raising-funds-using-defi/main/images/augmented_bonding_curve.png" />

`Source: https://medium.com/giveth/deep-dive-augmented-bonding-curves-3f1f7c1fa751`

The Hatch Phase is designed to allow initial contributors (founding members, devoted contributors, initial investors, etc.) to participate in a hatch sale. The purpose of this phase is to gather contributors and pool capital. A percentage of the capital is put into the Reserve Pool and used to mint tokens and determine the initial spot price during the Open Phase. The remaining capital in the Funding Pool is un-bonded and can be distributed as real capital outside of the bonding curve.

In a typical bonding curve system, the tokens can be burned at any time. However, in an augmented bonding curve system, the tokens minted during the Hatch Phase are locked and cannot be burned. This is to prevent any early speculation or arbitrage that could affect the stability of the Reserve Pool. It's important to have funds locked early on in the system to make sure that the capital in the Funding Pool is allocated to community initiatives, research projects and development milestones that will help the commons grow.

Once the goal for the Hatch Sale is reached, the new tokens go into a reserve pool where they can be bought or sold according to the bonding curve. The Hatchers tokens are gradually unlocked through this vesting process.

Whenever tokens are burned, an exit tax is enacted on liquidation. As members "cash out" and liquidate their funds, a small percentage of their returns are sent back into the funding pool, allowing for the simultaneous funding of the commons while contributors are earning returns. This means that the system always benefits - even if speculators are just looking to make a quick return.
 
### References
- https://hackernoon.com/what-are-bonding-curve-offerings-xi2k34bm
- https://dev.to/ceonyema/bonding-curve-offering-an-efficient-and-transparent-funding-model-4oae
- https://www.linumlabs.com/articles/bonding-curves-the-what-why-and-shapes-behind-it
- https://yos.io/2018/11/10/bonding-curves/
- https://medium.com/molecule-blog/designing-different-fundraising-scenarios-with-sigmoidal-token-bonding-curves-ceafc734ed97
- https://blog.goodaudience.com/rewriting-the-story-of-human-collaboration-c33a8a4cd5b8
- https://medium.com/giveth/deep-dive-augmented-bonding-curves-3f1f7c1fa751
- https://medium.com/aventus/token-bonding-curves-683b8b309c18
 
 **Liquidity Mining**        
Liquidity mining and yield farming are two terms that are often used interchangeably in DeFi. 

There are currently more than 50 DEXs and 50 lending and borrowing protocols, but only a few of each have achieved significant adoption. These platforms face a chicken and an egg problem, i.e. the more liquidity (funds) they have, the better the trade will be, and the more users will come to their protocol, which will further increase the funds and liquidity on the protocol.

Not just the amount of a crypto currently, but also the number of crypto currencies supported on a protocol also matters a lot. So to attract investors to bring money, most of these protocols offer rewards and share percentage of their fees. Rewards offered to the protocols are mostly the percentage of the trading fee and rewarding their native token. For example, 0x protocol offers ZRX tokens as rewards to its investors.

In the summer of 2020 and in 2021, we saw an influx of new projects offering investors and users huge rewards in order to attract them to their protocols. Most of these projects are in competition with one another, so investors have been able to take advantage of this by moving their funds around to different protocols and earning high rewards. As the rewards decreased or if another platform offered more attractive rewards, investors moved their funds again.

## Drawbacks of Liquidity Mining
There are several drawbacks to attracting liquidity simply by giving native tokens in exchange:
1. The liquidity providers are not motivated to help the protocol grow in the long term, so they may move to other protocols that offer better short-term rewards.
2. By giving away native tokens, protocols increase the total supply of their tokens in the market, which can cause prices to drop.
3. Even after providing heavy rewards, the investors remain in full control of the liquidity and can choose to leave the protocol at any time.

There are two common designs that different projects have adopted to combat this problem:

1. **Protocol Owned Liquidity** - Using this protocols sell their native tokens in the form of bonds at a discounted price in exchange for the needed assets. Bonds generally have a maturity date or vesting schedule towards distribution of native tokens. This mechanism is covered in detail in one of the following chapters. 

2. **veToken Model** - The veToken Model is a way of distributing newly minted tokens to investors who buy the native token of the project and lock it up for a certain period of time. This act of locking up the token proves that the investor believes in the long term success of the protocol and shows their commitment to the project. This model was first introduced by Curve protocol. 
 **Staking**        

## Background
Most enterprises need coverage for unforeseen events that could lead to financial losses, and this coverage is typically provided by insurance providers or investors. However, with the advent of decentralized finance (DeFi) protocols, it is now possible for anyone to stake/provide their funds to be used for the coverage of such losses. In return, the protocols usually reward these investors with either their native currency or some other form of compensation, in order to account for the risk they take by staking their funds.

## What is Staking?
Staking is the process of holding and locking up digital assets, such as cryptocurrencies, as a means of providing security for a protocol. By staking their assets, investors can earn rewards in the form of new tokens, interest, or other incentives. The specifics of staking can differ depending on the protocol, but it is generally a way for users to earn a return on their crypto assets while supporting the project.

## Examples
Following are two of the many examples where protocols using staking mechanism to raise funds

#### **Aave** 
The Aave Safety Module (SM) is a Smart Contract-based component that allows Aave holders to lock their tokens. This locked AAVE will be used as a way to help mitigate any Shortfall Events that may occur within the money markets of the Aave ecosystem. A Shortfall Event is defined as a deficit, and the interpretation or occurrence of such an event is subject to Protocol Governance vote.

If a Shortfall Event occurs, part of the locked AAVE is auctioned off on the market to be sold in order to cover the deficit that occurred. The Safety Module has a built-in backstop mechanism in place to prevent an excess flow of AAVE into the open market, which would further reduce the value of AAVE. Participants who lock AAVE into the Safety Module are effectively accepting the possibility of a Shortfall Event occurring, in exchange for receiving rewards in the form of Safety Incentives.

#### **Sherlock** 
When you stake USDC with Sherlock for a fixed term(6 months, 12 months etc.), you earn a market-leading APY in exchange for the risk that your funds could be used to pay out an exploit at a covered protocol. The APY for a staker is made up of three streams:
1) Premiums from protocol customers
2) Interest earned from depositing staker funds into yield strategies (Aave, Compound, etc.)
3) Incentive rewards paid in SHER (Sherlock’s governance token) 
 **Bonds**        
Bonds in DeFi are quite different from Traditional Bonds

### Traditional Bonds
A bond is a debt security, similar to an IOU. Borrowers issue bonds to raise money from investors willing to lend them money for a certain amount of time.

When you buy a bond, you are lending to the issuer, which may be a government, municipality, or corporation. In return, the issuer promises to pay you a specified rate of interest during the life of the bond and to repay the principal, also known as face value or par value of the bond, when it "matures," or comes due after a set period of time.

### DeFi Bonds
There is a lot of difference between bonds in DeFi and traditional bonds, just like there is a lot of difference between tokens and stocks. In some cases, projects might just be using the name "bond" for particular offerings, but the mechanics can be totally different from traditional bonds.

There are a few common mechanics that we often see being used in bonds as a way for DeFi projects to raise capital, these include:

1. **Exchange of Native Token**: In return for selling their native token, projects will ask for a stable token or one that is less volatile in exchange.
2. **Discount on Tokens**: To make the bonds more appealing, projects will sell them at a 
3. **Protocol owned Liquidity**: This is often used when a project needs to gain access to various tokens that are utilized as part of the product. For instance, to demonstrate the full potential of a Decentralized Exchange or Lending & Borrowing, protocols require access to a great deal of liquidity of different tokens.
4. **Secondary Markets**: Most of these bonds can be sold at a secondary market place, so the investor doesn't have to wait for the bond to mature.

In the next chapters, we will be looking at a couple of protocols that provides ability to create and sell bonds. 
 **Other Techniques**        
## Quadratic Funding

The Quadratic Funding mechanism, created by Glen Wyel at Microsoft and Vitalik Buterin, the founder of Ethereum, is a crowdfunding campaign in which dollars are allocated from a central matching pool to projects that are more democratically supported instead of those that receive more capital. This system is designed to reduce the power of whales (large investors) and favor democracy over plutocracy (a form of government in which the wealthy rule).

Example: If you raise a grant that gets $100 from 100 contributors, and I raise a grant that gets $100 from 1 contributor, despite both grants being donated $100, you will get 99% of the matching pool. This is a great mechanism because it is a collective intelligence mechanism that routes money to where the  “poor and the many” have an advantage over the rich and the few.

You may give "only" a dollar, but really you are part of building an aggregate signal of what public goods folks want to see funded. Problems like sybil attacks and the need to raise matching pool funds can be mitigated by using a one person: one vote identity style. 

## Retroactive Public Goods Funding 
Optimism is trying to do public goods funding retroactively by creating a committee of experts. They're taking revenue from the Optimism network and using it to pay the committee for their time researching which things in the past have delivered value to the ecosystem. The idea is that more talent will be directed toward developing public goods funding in the present based on the assurance that they will be rewarded for it in the future.

## References
- https://medium.com/giveth/coordination-mechanisms-notes-from-a-conversation-with-griff-green-kevin-owocki-af95f3e831b1
- https://youtu.be/qyd7mvQmn5I?t=1220
- https://youtu.be/qyd7mvQmn5I?t=1680 
 **Whale Problem**        
# Add problems related to having whales  
 **Regulations**        
When issuing tokens it is very important to be aware of different regulatory implications. Here we try to touch upon some of the most important points

## U.S. Securities and Exchange Commission (SEC)
In the United States, cryptocurrencies have received a lot of attention from both federal and state governments. The SEC typically has authority over the issuance or resale of any security token or other digital asset that constitutes security.

The SEC has been unequivocal in its opinion that even if a token issued in an ICO has utility, the token will still be deemed a security that is subject to the Securities Act if it meets elements of the Howey test.

Securities such as stocks and debt instruments, and also investment contracts, are under the direction of the SEC. Derivatives such as futures and swaps pertaining to commodities are under the oversight of the CFTC, unless those commodities are securities.

The future of cryptocurrency regulation is still an open question.

## Howey Test
The Howey Test is derived from a 1946 Supreme Court ruling in the case of the SEC v. W.J. Howey Co., which has been reaffirmed by the courts several times. Under the Howey Test, a transaction is considered a security if the following four criteria are met:
- Money is invested.
- There is an expectation the investor will earn a profit.
- The investment is in a common enterprise.
- Profits are generated via the efforts of others.

## Notable Regulations
Some of the most crucial legal frameworks that help you to fundraise from retail or private investors to offer you approval and remain compliant include the following.
1. **Reg CF** - Reg CF permits non-accredited (retail) investors to purchase private companies up to a certain limit depending on either their net-worth or annual income, helping businesses raise up to $5 million per year.
2. **Reg A** - Regulation A Tier 2 (the Mini-IPO/Reg A) is a less demanding variation of initial public offering (IPO). It's less regulated and can be used to raise up to $75 million every 12 months. It enables retail investors to invest alongside accredited and institutional investors
3. **Reg D** - Regulation D, Rule 506 allows accredited investors to invest in private investment firms without an upper limit and without having to go public.



  
 

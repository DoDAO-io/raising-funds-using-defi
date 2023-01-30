## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Bond Protocol
 
 **What is Bond Protocol?**        
### What is Bond Protocol?

Bond Protocol (Olympus Pro) is a platform that allows any project to acquire liquidity for their DAO or protocol by selling bonds. Bond Protocol is, at its core, a service for protocols wishing to use bonds in their emissions programmes with minimal overhead and maximum impact. They give infrastructure, experience, and exposure to partners. Projects need only bring a token and a goal.

Protocols can accumulate the critical infrastructural liquidity that they typically service through liquidity mining through bonds. Instead of renting that liquidity (sometimes at exorbitant interest rates), they simply buy it, transforming a value-draining permanent expense into revenue-generating assets that enable the rest of the platform's functioning. This is a significant change from the traditional way of liquidity mining, where projects rent liquidity with rewards.

The flow of funds can be simplified as follows:
![Flow of funds in traditional model](https://github.com/DoDAO-io/raising-funds-using-defi/blob/4f970f73ec8f4da8e093487828a261be6facce7c/images/flow_of_funds_in_traditional_model.png?raw=true) `Reference: https://docs.bondprotocol.finance/`

In the traditional model, projects pay tokens from their treasury over a set period of time to rent liquidity and the attention of liquidity providers (LPs). Often, when these rewards end, LPs simply move on to the next farm, making the liquidity mining event a sunk cost with little to show for. With Bond Protocol, projects can make the flow of funds circular and create a symbiotic relationship with profit seekers and their community alike. As projects use the bonding mechanism to improve their liquidity, that liquidity makes its way back to the project's treasury and becomes a permanent, income-producing asset. In other words, liquidity mining through Bond Protocol is no longer a sunk cost, and the project now has full control over the liquidity they paid for.
![Flow of funds using bonding](https://github.com/DoDAO-io/raising-funds-using-defi/blob/4f970f73ec8f4da8e093487828a261be6facce7c/images/flow_of_funds_using_bonding.png?raw=true) `Reference: https://docs.bondprotocol.finance/`

By flipping the traditional model on its head, projects not only benefit, but so do their communities. Community members can rest easy knowing that the liquidity for the token they support won't disappear overnight when incentives dry up. They'll also be much happier knowing that the project is receiving an income-producing asset in return for token rewards rather than renting mercenaries. These two major improvements create a much healthier ecosystem around each token and allow young projects to thrive.

  
 
 **What is Bonding?**        
### What is Bonding?

Bonding is a process in which a user can sell an asset, such as a Quote Token, in a bond market created by an issuer, in exchange for a discounted Payout Token at a later date. To encourage users to sell to the protocol rather than the open market, bonds are offered at a discounted rate, and they also have a vesting period to prevent users from selling all the discounted tokens at once for a quick profit.

A continuous [Dutch auction](https://medium.com/@Bond_Protocol/auctions-what-the-dutch-80e4bb3ee7ad) is used to price the bonds, and the price is determined by the supply and demand of bonds in the market. The bond price goes up when there is more demand, and goes down when there is less demand. This mechanism provides a real-time reflection of the bond price in the market. As a result, bonding is a highly competitive space, with participants competing to get the largest discount.

Below image is a good visualization of how it works: ![Dutch Auction](https://github.com/DoDAO-io/raising-funds-using-defi/blob/4f970f73ec8f4da8e093487828a261be6facce7c/images/dutch_auction.png?raw=true) `Reference: https://medium.com/@Bond_Protocol/auctions-what-the-dutch-80e4bb3ee7ad`

There are several benefits of bonding, such as allowing a protocol to accumulate their own liquidity. 

Protocol Owned Liquidity (POL) allows a protocol to provide guarantees to users that there is always sufficient liquidity for normal market operations. Without POL and relying on external liquidity providers, in distress market conditions, liquidity is often pulled from the protocol, exacerbating the situation with less exit liquidity (liquidity death spiral).

Another benefit is that POL transforms liquidity from a liability to a revenue source. Every swap transaction in a pool contributes a 0.3%/0.25% (Uniswap/Sushiswap) fee to the LPs. With POL, as liquidity is permanently locked in the treasury, these fees provide a constant source of revenue for the protocol. 

Additionally, POL allows for additional yield farming opportunities, such as the Onsen program offered by Sushiswap, where protocols can have their liquidity pair listed for SUSHI rewards. Once successfully listed, the protocols can deposit their SLP tokens into the Onsen menu and farm SUSHI tokens.
 
 **Types of Bonds**        
### Bond market participants

- **Issuer**: Create bond market by defining Payout Token to be paid out and Quote Token to receive. - **User**: Purchase future-dated Payout Token with Quote Token at the current market price and receive Bond Token to represent their position while their bond vests. Once the Bond Token vest, it can be redeemed for the Payout Token.

### Types of Bonds

- **Fixed-term bonds**
  * Each position vests a set amount of time after purchase (based on UTC timestamp)
  * Tokenized as ERC1155

- **Fixed-expiry bonds**
  * All purchases vest at a specific timestamp
  * Tokenized as ERC20
  * Minimum 3 days vesting to maximum 9 months (on Bond Protocol front-end)
 
 **Advantages**        
### Advantages of Bond Protocol
- **Increase project runway, reduce insolvency risks**: Most protocols are over-exposed to their native governance token, with most treasuries having <10% diversification. Issuing bonds allows funds for development and investment in strategic initiatives to increase protocol viability and longevity. - **Acquire liquidity at lower long-term cost**: Protocols pay a lot to rent liquidity via inflationary incentives paid in their native governance token. High incentives paid to mercenary capital can create negative feedback loops that destroy value for the protocol and token holders. - **Permissionless**: Anyone can create a bond market! Bond Protocol is self-contained and trustless, just like you would expect from a DeFi protocol. When you launch a bond on our marketplace, you are in complete control. You can choose to receive and bond any ERC20 token, including base assets and LP tokens. The vesting period, bond capacity, and market duration can be tuned to suit your protocol’s needs. - **Composable**: Bond purchasers receive Bond Tokens (tokenized bonds) that represent their positions which allow for the creation of secondary markets. With the introduction of tokenized bonds, a new range of opportunities is unlocked in DeFi. Bonds can be used as collateral, exchanged between wallets, or even used in governance.  - **Modular**: Bond Protocol's contract architecture makes it easy to add new bond assets and auction interfaces. Protocols will be able to select from a variety of bond markets that best suit their unique attributes. Initially launched with two types of bond vesting, Fixed-Term (ERC1155) and Fixed-Expiry (ERC20). Fixed-Term bonds are most similar to classic Olympus bonds, with their maturity set a fixed number of days from purchase (ex: 14 days). With Fixed-Expiry bonds, on the other hand, all bonds issued from that market mature on a specific date (ex: Dec-31).
![Bond Protocol Architecture](https://github.com/DoDAO-io/raising-funds-using-defi/blob/4f970f73ec8f4da8e093487828a261be6facce7c/images/bond_protocol_architecture.png?raw=true) `Reference: https://docs.bondprotocol.finance/`
 
 **Growth and Adoption**        
### Growth and Adoption of Bonds Protocol
Bond Protocol has achieved tremendous success through bonds. The protocol amassed over $150 million in assets in its first six months. This is greater than many protocols' TVL, and it will never have to pay for them again. Not only that, but the majority of these assets are productive; rather than costing the protocol money, they generate it.
Olympus changed the game with its bonding mechanism to acquire liquidity. Olympus-style bonds have been around for almost [18 months](https://olympusdao.medium.com/introducing-olympus-pro-d8db3052fca5) and have been used by over 50 protocols on 7 chains. Bonding allows savvy protocols to generate on-demand liquidity using their governance tokens. The total bonded value stands at [$18 million](https://app.bondprotocol.finance/#/issuers) as of Jan 2023 with [750+](https://app.bondprotocol.finance/#/issuers) total bonds.
 
 **References**        
- https://bondprotocol.finance/ - https://docs.bondprotocol.finance/ - https://medium.com/@Bond_Protocol - https://eyesoftheworld.substack.com/p/olympus-pro
 
 

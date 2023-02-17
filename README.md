# 2023-Medium-Risk-Findings-Sherlock<br>
<p align="center">
                                <a href="https://www.ajna.finance/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/as16x/2023-Midium-Risk-Findings-Sherlock/main/Sherlock/Ajna.jpg" width="60" height="60" alt="Javascript" /></a></p>    
                                
---
* [[M-01] Buypunk function of Cryptopunks in ERC721Pool is used incorrectly - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/163)
* [[M-02] ERC721Pool taker callback misreports quote funds whenever there was collateral amount rounding - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/162)
* [[M-03] Anyone can transfer approved LP tokens - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/156)
* [[M-04] Incorrect MOMP calculation in neutral price calculation - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/148)
* [[M-05] Extraordinary proposals can receive more tokens than eligible - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/124)
* [[M-06] Claiming rewards from a future not yet existing epoch prevents claiming rewards for those epochs later on - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/124)
* [[M-07] Calculating new rewards is susceptible to precision loss due to division before multiplication - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/121)
* [[M-08] Claiming accumulated rewards while the contract is underfunded can lead to a loss of rewards - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/120)
* [[M-09] [M] Incorrect Validation in Pool.sol#transferLPs lead to a DOS attack - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/116)
* [[M-10] Adversary can grief kicker by frontrunning kickAuction call with a large amount of loan - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/111)
* [[M-11] Settled collateral of a borrower aren't available for lenders until borrower's debt is fully cleared - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/104)
* [[M-12] Deposits are eliminated before currently unclaimed reserves when there is no reserve auction - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/102)
* [[M-13] Flashloan end result isn't controlled - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/101)
* [[M-14] Interest rates can be raised above the market as a griefing, disabling the pool - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/100)
* [[M-15] Interest rate for pool is bounded wrongly - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/96)
* [[M-16] Auction timers following liquidity can fall through the floor price causing pool insolvency - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/76)
* [[M-17] If borrower or kicker got blacklisted by asset contract their collateral or bond funds can be permanently frozen with the pool - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/75)
* [[M-18] user can drawDebt that is below dust amount - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/70)
* [[M-19] Quadratic voting tally done wrong - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/64)
* [[M-20] CryptoKitty and CryptoFighter NFT can be paused, which block borrowing / repaying / liquidating action in the ERC721Pool when borrowers still forced to pay the compounding interest - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/34)
* [[M-21] Minting an NFT with a position on the same bucket as a previously minted NFT changes its deposit time - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/19)
* [[M-22] Memorializing an NFT position on the same bucket of a previously memorialized NFT locks redemption - ajna.finance - 2023-Feb](https://github.com/sherlock-audit/2023-01-ajna-judging/issues/13)

<p align="center">
                                <a href="https://ag0.gitbook.io/cooler-loans/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/as16x/2023-Midium-Risk-Findings-Sherlock/main/Sherlock/01UO5m5.jpeg?raw=true" width="60" height="60" alt="Javascript" /></a></p>    

* [[M-01] Cooler.roll() wouldn't work as expected when newCollateral = 0. - Cooler loans - 2023-Feb](https://github.com/sherlock-audit/2023-01-cooler-judging/issues/320)
* [[M-02] Loan is rollable by default - Cooler loans - 2023-Feb](https://github.com/sherlock-audit/2023-01-cooler-judging/issues/265)
* [[M-03] Repaying loans with small amounts of debt tokens can lead to underflowing in the roll function - 2023-Feb](https://github.com/sherlock-audit/2023-01-cooler-judging/issues/263)
* [[M-04] Dust amounts can cause payments to fail, leading to default - Cooler loans - 2023-Feb](https://github.com/sherlock-audit/2023-01-cooler-judging/issues/218)
* [[M-05] DAI/gOHM exchange rate may be stale - Cooler loans - 2023-Feb](https://github.com/sherlock-audit/2023-01-cooler-judging/issues/217)
---
<p align="center">
                                <a href="https://sentiment.xyz" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/as16x/2023-Midium-Risk-Findings-Sherlock/main/Sherlock/Sentiment%20Update.jpg" width="60" height="60" alt="Javascript" /></a></p>    
                                
* [[M-01] Tokens not owned by an account can be added as an asset to the account - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/26)
* [[M-02] Risk with Liquidation - Because of partnership requirement, caller may be unable to redeem during liquidation making it less likely for them to be willing to perform the liquidation - entiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/20)
* [[M-03] PreviewRedeem may under-price the value of the asset - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/19)
* [[M-04] No check if Arbitrum L2 sequencer is down in Chainlink feeds - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/16)
* [[M-05] GMX Reward Router's claimForAccount() can be abused to incorrectly add WETH to tokensIn - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/10)
* [[M-06] Using one controller for two addresses could risk signature collisions - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/9)
* [[M-07] All Rage Trade functions allow sending tokens to a different address, leading to incorrect tokensIn - sentiment.xyz - 2023-Jan](https://github.com/sherlock-audit/2023-01-sentiment-judging/issues/5)<br>
---
<p align="center">
                                <a href="https://uxd.fi" target="_blank" rel="noreferrer"><img src="https://github.com/as16x/2023-Midium-Risk-Findings-Sherlock/blob/main/Sherlock/UXD%20Protocol.jpg?raw=tru" width="60" height="60" alt="Javascript" /></a></p>    
                                
* [[M-01] `rebalanceLite` should provide a slippage protection - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/429)
* [[M-02] `PerpDepository._rebalanceNegativePnlWithSwap()` shouldn't use a `sqrtPriceLimitX96` twice. - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/425)
* [[M-03] Vulnerable GovernorVotesQuorumFraction version - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/423)
* [[M-04] Deposit and withdraw to the vault with the wrong decimals of amount in contract `PerpDepository` - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/402)
* [[M-05] PerpDepository#_rebalanceNegativePnlWithSwap fails to approve vault for quote deposit - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/372)
* [[M-06] Inaccurate Perp debt calculation - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/346)
* [[M-07] Rebalancing a negative Perp PnL via a Uniswap V3 token swap is broken due to the lack of token spending allowance - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/339)
* [[M-08] Redeeming all UXD tokens is not possible if some have been minted via Perp quote minting - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/338)
* [[M-09] Price disparities between spot and perpetual pricing can heavily destabilize UXD - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/305)
* [[M-10] The `FullMath` library is unable to handle intermediate overflows due to overflow that's desired but never reached - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/273)
* [[M-11] PerpDepository#_placePerpOrder miscalculates fees paid when shorting - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/271)
* [[M-12] PerpDepository.netAssetDeposits variable can prevent users to withdraw with underflow error - uxd.fi - 2023-Jan](https://github.com/sherlock-audit/2023-01-uxd-judging/issues/97) 
---
<p align="center">
                                <a href="https://illuminate-app.vercel.app/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/as16x/2023-Midium-Risk-Findings-Sherlock/main/Sherlock/Illuminate.png" width="60" height="60" alt="Javascript" /></a></p>    
                                
* [[M-01] ERC5095 has not approved MarketPlace to spend tokens in ERC5095 - illuminate-app - 2023-Jan](https://github.com/sherlock-audit/2023-01-illuminate-judging/issues/23)
* [[M-02] Protocol fees not taken on premium - illuminate-app - 2023-Jan](https://github.com/sherlock-audit/2023-01-illuminate-judging/issues/22)

# 2023-Medium-Risk-Findings-Sherlock<br>
---
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

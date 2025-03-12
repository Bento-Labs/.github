# Redemption

bentoX assets can be redeemed at any time for any eligible asset or basket of collateral assets in the reserve. Users should have a way to exit at any time, and so this feature is available in any conditions. bentoX tokens are redeemable on a 1:1 basis for USD/ETH/BTC if the collateral ratio is healthy.

bentoX tokens offer flexible redemption options:

1. Users can instantly withdraw the basket of yield-bearing tokens that represent the deposits in various yield-generating strategies, such as aUSDC, sDAI, or sUSDe. Alternatively, users can withdraw the underlying collateral assets (e.g., USDC, USDe, DAI) after the unbonding period required by some strategies.
2. Users can redeem bentoX tokens for any underlying collateral asset. Bento uses an intent-based mechanism where solvers calculate the optimal route for converting the basket of yield-bearing tokens or collateral assets into a single asset that the user wishes to withdraw. Solvers can also provide external liquidity to fulfill user withdrawal requests by purchasing user shares and later redeeming them for profit.
3. Users have the option to sell bentoX tokens on secondary markets for any desired asset. Since bentoX tokens are fully redeemable in the primary market, their 1:1 peg with underlying assets is maintained, supported by arbitrage opportunities.

Bento’s redemption module enables at all times and in any circumstance users to redeem bentoX tokens for a proportion of reserve assets minus a fee that depends on the overall collateral ratio of the system. This action is meant to be the privileged method of interaction with the protocol during black swan events (like a depeg of one of the collateral assets in the system).

There is no fee when the collateral ratio is greater than or equal to 100% but starts increasing as the collateral ratio decreases below 100% in black swan events like depegging of any underlying collateral or any of the underlying protocols are exploited. The goal is to disincentivize runs and attacks on the currency peg, while enabling users to exit, but rewarding users that wait for a transitory downturn to pass.

Users who still want to exit when the protocol gets badly collateralized may still exit, but by doing so they are re-collateralizing the protocol, thus leaving better off the users who remained in the system. Below a certain level of collateral ratio, the fee can go back to 0 to enable all users to exit at the fair value of the reserves when the protocol is in an irremediably bad health.

Importantly, even if bentoX holders decide to exit, Bento provides rational reasons to bet on the token returning to its target price, as the redemption price autonomously recovers back toward peg as outflows equilibrate back toward zero or the reserve recovers (e.g., through yield, insurance fund, BENTO emissions).\

# Minting

Users can deposit the collateral assets on any of the chains supported by Bento protocol to instantly mint bentoX or bentoX+ directly on any chain seamlessly. Once minted, bentoX tokens can be bridged across chains without friction.&#x20;

bentoX tokens offer flexible minting options:

1. bentoX tokens can be minted directly from any eligible collateral assets, provided that the price deviation of the asset from its target value (e.g., $1 for stablecoins or the Net Asset Value (NAV) for other collateral assets in USD/ETH/BTC) remains within a reasonable range. If an asset becomes de-pegged, minting with that asset is temporarily disabled. The protocol uses a zapper function to automatically convert deposited assets into the required basket of underlying collateral assets via DEXs or DEX aggregators, which are then deployed into yield-generating strategies.&#x20;
2. Users may also deposit the entire basket of underlying collateral assets directly, allowing for instant minting of bentoX tokens without incurring slippage or fees.
3. Alternatively, bentoX tokens can be acquired through secondary markets on DEXs using any asset, providing flexibility for users who prefer to trade on the open market.

bentoX tokens are minted on a 1:1 basis for USD/ETH/BTC with the eligible deposit assets at price:

Min (Price, 1 USD) for bentoUSD

Min (Price, 1 ETH) for bentoETH

Min (Price, 1 BTC) for bentoBTC

Here, the Price represents the market value of the deposit assets, denominated in USD, ETH, or BTC, and is calculated using aggregated oracle price feeds.

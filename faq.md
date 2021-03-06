# FAQ

## Trading/Listing, Supply Cap

### 1. What is ACS and what is ACSI? What are their core products?

* ACS is the native token of ACryptoS \(connected with all the Vaults farming on PCS and Venus Protocol\), while ACSI is the native token of the StableSwap.
* The core product of ACS is yield farming optimizers for multiple types of tokens.

  The core product of ACSI is the StableSwap, which is an automated market maker.

### 2. Where is ACS listed and traded?

* ACS is currently listed on [Coinmarketcap](https://coinmarketcap.com/currencies/acryptos/), [Coingecko](https://www.coingecko.com/en/coins/acryptos), [Defistation](https://www.defistation.io/acryptos), [DappRadar](https://dappradar.com/binance-smart-chain/defi/acryptos), [MATH dApp Store](https://mathdapp.store), [Coinbase Prices](https://www.coinbase.com/price/acryptos) and traded on the [Pancakeswap Exchange](https://exchange.pancakeswap.finance/#/swap?outputCurrency=0x4197C6EF3879a08cD51e5560da5064B773aa1d29) and on [Hotbit](https://www.hotbit.io/exchange?symbol=ACS_USDT) (low volume on Hotbit, be careful).

### 3. What is the maximum supply cap?

* The maxium supply cap for ACS is 1,888,888.
* There is an on-going vote for capping ACSI at 1,888,888.

### 4. Is there a buy-back program?

* Yes. The system is designed to constantly buy-back ACS \(using the withdrawal fee + the performance fee\), and then those ACS are distributed to the acsACS holders.
There are also constant buybacks for ACSI, using 50% of the swap fee from the StableSwap, and then those ACSI are distributed to the acsACSI holders.

### 5. How many tokens are minted per day?

* There was aconstant daily emission rate of ~3746 ACS tokens:

  ~2560 ACS to the farms

  +33.33% to the ACS Vault \(~853\)

  +10% reward to the dev team \(~256\)

  +3% to the treasury \(~77\)

  The genesis mining is ~8888 ACS.

* After the first emission cut (15 Feb 2021), the emission was reduced by 18.65%.

### 6. Are the tokenomic models of ACS and ACSI sustainable?

* For ACS: the performance and withdrawal fees gained from providing the yield farming services to users are used to buy-back ACS from the market and then the ACS is redistributed to the ACS Stakers. This ensures a sustainable future of ACS.
* For ACSI: 50% of the fees gained from stablecoin swap are used to buy-back ACSI from the market and then the ACSI is redistributed to the ACSI Stakers. This ensures a sustainable future of ACSI.

### 7. What is the vision of ACS and ACSI

* The vision of ACS is to be the YFI on the Binance Smart Chain \(BSC\).
* The vision of ACSI is to be the Curve \(Crv\) on the Binance Smart Chain \(BSC\).

## Security

### 1. Are the contracts behind a timelock?

* Yes, all contracts are behind a timelock. For more details, please refer to [Security & Risks](https://docs.acryptos.com/security-and-risks).

### 2. Are the contracts verified?

* Yes, all contracts have [verified and published source codes on BscScan](https://app.acryptos.com/contracts/).

### 3. Is the project audited?

* Yes. The project has been audited.
 - By DefiYield on 28 Jan 2021. Check the [full audit report here](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210128-defiyield.info.pdf).
 - By Hacken on 18 Feb 2021. Check the [full audit report here](https://github.com/acryptos/acryptos-protocol/blob/main/audits/20210218-Hacken-ACryptoSFarmV2.pdf).

## Fees

### 1. Is there a Deposit fee?

* No.

### 2. Is there a fee on the first Stake?

* ACS Farms: No. However additional staking/unstaking triggers the harvest and the 0.5 ACS fee (this will be changed soon with the migration to farms v2.). 
  Currently there is a promo and the harvest fee is 0 until 25 Feb 2021.
 

* ACSI Farms: No.

### 3. What are the withdrawal fees?

* There is a 0.5% withdrawal fee. This fee is applied on all vaults \(except the ACS Vault and the ACSI Vault\).
* For the ACS Vault and the ACSI Vault, the withdrawal fee is 10% \(applied only on the amount you withdraw\).

  Example: If you have 1000 ACS in the ACS Vault, and you decide to withdraw 100 ACS, the fee will be 10 ACS.

### 4. What are the harvest fees on the farms?

* The harvest fee is 0.5 ACS on the ACS farms, and 5 ACSI on the ACSI farms \(currently both harvest fees are 0, promo period during LNY\).

  Note: Clicking the stake/unstake button also triggers the harvest \(only on the ACS Vaults&Farms v1\).

  If you harvest when your Pending ACS is less than 0.5 ACS, your Pending amount will reset to 0 \(currently the harvest fee is 0 ACS, promo period during LNY\).

### 5. What are the performance and the workers fee?

* The performance fee is 5% and the workers fee is 0.3% \(both are applied only on the profit\).

  These fees are already reflected in the shown APR.

### 6. Which fees are visible and which are already included in the APR?

* The vault’s performance fee and workers fee \(5% + 0.3%\) are already included in the APR you see, so no need to do any math on that.
* You only need to be careful with the farms’ harvest fee \(0.5 ACS - currently 0 ACS, promo period during LNY\), the vaults' withdrawal fee \(0.5%\), and the withdrawal fee on the ACS Vault \(10%\).

### 7. What are the fees on the StableSwap?

* The exchange fees are set to 0.04%, which is almost 10 times cheaper than the 0.3+% charged by all the other UniSwap and SushiSwap clones.

  All this is possible thanks to Curve’s [specialized algorithm tailored for trading of stablecoins and other pegged assets](https://www.curve.fi/stableswap-paper.pdf).

### 8. What is the difference between APR and APY?

* APR reflects the simple interest rate over a year’s time \(APR/365\), while APY describes the rate with the effect of compounding.

## Technical and UI

### 1. What is the difference between Deposit \(Vault\) and Stake \(Farm\)?

* When you Deposit tokens to a Vault, the deposited tokens start to auto-compound right away. 
* When you Stake those same tokens, you start earning ACS.

### 2. Does ACS auto-compounds?

* Yes, ACS auto-compounds in the ACS Vault.

  If you have Pending ACS in one of the other Vaults, you first need to harvest them and transfer them to the ACS Vault.

### 3. How the auto-compounding works \(and what is the Workers tab\)?

* Currently there is a bot that automatically harvests each Vault at least once a day. 
* There is also the Workers tab, where anyone can manually harvest each Vault \(and get the associated fee\).

  The Workers tab is just a backup, the normal user does not have to use it.

### 4. When does the ACS buy-back happen?

* The ACS buy-back happens when the bot harvests the ACS Vault.

  When this happens, all the tokens gained from performance and withdrawal fees are first transferred to BNB, and then to ACS.

  Then the ACS is distributed to the ACS Vault stakers \(acsACS holders\).

### 5. How does the Venus strategies work?

* By supplying an asset and borrowing the same asset to resupply with.

  Example: Supply BNB, borrow BNB, supply more BNB, borrow more BNB, and repeat.

  With this method we are earning both supply and borrow rewards, with minimal liquidation risk as we are using a single asset.

### 6. Why does the APR on some Vaults show weird numbers?

* The UI shows the average APR of the last 3 days.

  So if a Vault is new, the numbers could be off.

### 7. I cannot find the “harvest” or “withdraw” button, where are they?

* The User interface \(UI\) is dynamic. The harvest button appears after you have at least 0.5 ACS Pending for harvest \(currently the harvest fee is 0, promo period during LNY\).
* If your assets are Staked, the Withdraw button appears after the Unstake.

### 8. What is ACS4USD and what is ACS4VAI?

* When you deposit Stable coins to the ACS4USD StableSwap, you receive ACS4
* When you deposit Stable coins to the ACS4VAI StableSwap, you receive ACS4VAI.

  Then you can then stake those ACS4 / ACS4VAI in the ACS4USD / ACS4VAI farms to earn ACSI.

## Governance and Voting

### 1. Is there a treasury?

* Yes. A treasury was formed to fund anything that adds value to the protocol, taking up to 3% of ACS emissions.

### 2. What is the main goal of the treasury?

* The treasury funds will be used to improve/add value the project \(marketing/pr/administration/management/audits/etc\).

### 3. Who controls the treasury?

* The treasury is controlled via governance.

### 4. Who can vote?

* ACS held in the ACS Vault and ACSI held in the ACSI Vault are our governance tokens. Voting weight is measured in ACS, using the prevailing ACS-ACSI exchange rate.

### 5. Where do I vote?

* You can vote on [the governance platform](https://vote.acryptos.com/#/acryptos/all).

### 6. Who can create a new vote/proposal?

* Anyone who holds at least 88 ACS.

### 7. Which governance platform is used for voting?

* We are using the well-established gasless [governance client](https://snapshot.page) by Snapshot Labs.


# Binance Futures Leaderboard API 

##### Welcome to the first Free API documentation for the Binance Public leaderboard API. 

The main use of this [leaderboard ](https://www.binance.com/en/futures-activity/leaderboard/top-ranking) is to check on Binance TOP futures traders, and see their position. 

I decided to startt documenting this API since binance don't want to.

### Leaderboard

```
https://www.binance.com/bapi/futures/v3/public/future/leaderboard/getLeaderboardRank
```
##### Parameters : 
```
{
  "isShared": true,
  "isTrader": false|true,
  "periodType": "DAILY|WEEKLY|MONTHLY|ALL",
  "statisticsType": "PNL|ROI",
  "tradeType": "DELIVERY|PERPETUAL"
}
```
Explaining : 
* `isShared` must be on True since it's asking to show all the traders that have public positions.
* `isTrader` can be enabled to display the traders having [**Copy Trading**](https://en.wikipedia.org/wiki/Copy_trading).
* `periodType` may have differents values depending on the results timeframe you want.
* `statisticsType` changes the results from **R**eturn **O**n **I**nvestment (%) to **P**rofits '**N** **L**osses ($)
* `tradeType` changes the trade type : Perpetual futures support up to 125x leverage, while delivery futures only support up to 20x leverage

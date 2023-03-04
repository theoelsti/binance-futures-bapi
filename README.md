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
  "isTrader": false,
  "periodType": "WEEKLY",
  "statisticsType": "ROI",
  "tradeType": "PERPETUAL"
}
```

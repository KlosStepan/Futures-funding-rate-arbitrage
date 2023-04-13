# Futures-funding-rate-arbitrage
We are working on a bot for gathering Bitcoin perp futures fee by hedging futures position with spot and collective negative fee.  

## Tech stack
- Node.js  

## Roadmap of program
- Integration with Binance
- Interface to buy/sell spot & long/short futures to be exchange agnostic
- Basic order execution from program - "strategy"
- Funding fees data download/analysis
- Normal (intended) strategy to check funding rates and open (short f & buy spot)  

## Proof of concept - analysis &/or issues
- Futures/Spot spread difference (might not be a problem if same for hedging over the course of 8h trade)
- Test on previous bull market, Bitcoin each 8h strategy short & buy
- (Long/sell) strategy as well - spot Bitcoin necessary for sell (!)
- Worst spreads when closing opposite positions over the course of bullrun
- Calculate potential compound over 2021 bullrun
- Advanced strategy - trade the most profitable pair each funding window (8h) and compound like this - test all previous things on this strategy as well
- Both sides during boring market, btc/most prof. pair  

## Links
- https://jamesbachini.com/futures-funding-rate-strategy/
- https://binance-docs.github.io/apidocs/futures/en/#mark-price

## Other stuff 
- https://www.coinglass.com/FundingRate
- Find good BTCPERP explanation, tldr; funding each 8h, fee based on demand either loners->shorters or other way around  
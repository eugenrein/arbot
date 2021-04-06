## Arbitrage finding bot

**Use at your own risk**  

Idea for the bot is to fetch tickers from multiple exchanges and compare them pairwise.
Differences in prices which cross a certain threshold consistitutes a arbitrage opportunity.

[Not yet implemented] Opportunities are further evaluated by fetching the orderbooks of
both exchanges and examining the buy/sell liquidity on both. Then you could present the potential percentage gains
for different order sizes.

If you can buy the asset for a lower price on one exchange than you can sell it on another exchange,
it's possible to earn money on the difference minus any trading fees. **However, some currencies may for a long time, or permanently trade at different prices on different exchanges, for example due to broken exchange wallets.**

There are two ways of taking advantage of price differences between exchanges:
- If you hold the asset on the exchange with higher price, you can sell the asset there, 
and buy it on the lower priced exchange, given that you own the quote currency at the lower priced exchange
- If you hold the asset on none of the exchanges, but got access to margin on the higher priced exchange, 
then you can short the asset on the higher priced exchange and buy it on the lower priced exchange. Then you'd 
wait for the prices to start trading closer to each other. **This exposes you to liquidation risk on the higher 
priced exchange.**

# Market-Microstrucure-and-Transaction-Costs
I investigated the relationship between market capitalisation and transaction costs.

The data contains the national best bid and offer prices (NBBO) for 117 stocks on October, 1, 2010.

First, my goal was to find the national best bid and offer price at the time of each trade.

Then, for buyer-initiated trades—i.e., when BuySell = “B”—I calculated the volume-weighted average transaction cost for the buyers for each the 117 stocks. Specifically, I calculated the transaction cost for each buyer-initiated trade, and then computed a weighted average of these transaction costs for each stock, using the numbers of shares traded as weights. The transaction cost is computed as a fraction of the benchmark price, where the benchmark price is the midpoint of the national best bid and offer prices at the time of the transaction. For example, if the national best bid and offer prices are $10.00 and $10.20, respectively, and a transaction of 200 shares occurs at $10.20, the transaction cost for this trade as a proportion of the benchmark price is (10.20 – 10.10)/10.10 = 0.99%, or 99 bps. Similarly, I then calculated the volume-weighted average transaction cost for sellers. Note that each trade shows up only once in the trade data—e.g., there isn’t a duplicated entry for the counterparty seller if it is a buyer-initiated trade.

Finally, I regressed the volume-weighted average buyer and seller transaction cost for each stock on the natural logarithm of its market capitalization.


I found that the transaction costs for both buyer and seller-initiated trades are decreasing as the log market cap increases. The financial intuition behind these findings could be that larger companies are more mature. This would lead to a small spread between the bid and ask price as the price does not move a lot. Thus, the midpoint would be closer to the trading price and we would find a lower transaction cost. Another explanation could be that large companies are more traded and thus, the liquidity risk for market makers is very low, allowing to have a smaller spread and again lower transaction costs. On the contrary, the spread would be higher for smaller stocks with less volume as the market-makers would need to be compensated for the higher liquidity risk.

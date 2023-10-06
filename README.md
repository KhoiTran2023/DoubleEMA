# DoubleEMA
if dip into zone, consider   
1: if break out of zone going up, buy   
2: if break out of zone going down, sell   
stop-loss below 20 EMA - risk   
profit-target: 1 x 20 EMA (experiment, risk to reward ratio)   
trailing stop loss?   
Experiment with different time frames   

Set up EMA, one on length 9 (sma) smoothing (9), one on length 20 (sma) smoothing (20), on (5 minute)
1. if 9 EMA is above 20 EMA, then it is uptrend, look to take a long position   
  1. if (1 minute) candle closes (below) 9 ema and (above) 20 ema.
  2. while loop to be interested in a trade until buy order is triggered or SL occurs (price goes a couple points below 20 EMA)
     1. if price breaks dip candle high by a couple of points then trigger buy order
     2. else wait for next second
  4. while buy order is in open position
     1. set SL as a couple points below 20 EMA after (10 minutes)
     2. set profit target as (1X) the SL 20 EMA to initial open position
        1. when either are triggered, close the position

5. else if 9 EMA is below 20 EMA, then it is downtrend, look for short position
   1. vice versa of long position

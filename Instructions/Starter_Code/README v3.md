# FINTECH-Challenge-14-Algorithmic-Trading

## Establish a Baseline Performance

*CONCLUSIONS - Baseline Trading Algorithm (3-months DateOffset, SMA short window = 4, SMA long window = 100):*

    From mid-2015 to mid-2018, the actual vs strategic returns did not diverge.  From mid-2018 onward, our trading algorithm started to outperform the actual returns.  

![Baseline Trading Algorithm - Actual vs Strategy Returns](Plot - Strategy vs Actual Returns.png)  


## Tune the Baseline Trading Algorithm

### DATE OFFSET

*Training set size change #1 - 6-months*

    The 6-month training set was very effective after the 2020 COVID crash.  I would argue for using a 6-month date offset going forward.  It took some additional time to learn and make mistakes, but this 6-month offset looks poised to generate good returns into the future.


*Training set size change #2 - 1-month* 

    The 1-month training set produced consistently higher returns that the actual returns, though the difference was small.  


*Training set size change #3 - 9-months*

    The 9-month training set produced very mixed results.  I would not advise using this date offset for our trading bot.



### SMA WINDOWS

*SMA window changes #1 - Short Window = 2, Long Window = 50*

    Lowering the short and long windows had a negative impact on returns.


*SMA window changes #2 - Short Window = 8, Long Window = 200*

    Doubling the short and long windows from the original (4 & 100) also produced negative returns.


*SMA window changes #3 - Short Window = 6, Long Window = 100*

    Changing the short window to 6, even while keeping the Long Window constant at 100, still produced worst results.



### FINAL TUNING

After a good deal of tuning, the best set of parameters was the following:

## Date Offset of 6-months
## SMA window changes #3 - Short Window = 8, Long Window = 100

![Baseline Trading Algorithm - Actual vs Strategy Returns](Plot - FINAL TUNING - Strategy vs Actual Returns.png)  







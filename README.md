# stockspredicter

#5/7/25
1. Incorporate earnings dates to be removed within 2 weeks
     a. Or could forecast earnings
2. Economic indicators
3. News indicators
     a. Twitter
     b. News
     c. Government officials news
     d. Fed rates
4. Email fix
5. update front end



how calculate.py works: 

 loop(path) --> path is the path to a directory, the loop function retursn a list of all the contents in the director 
            --> basically python's way of getting the result to 'ls' in linux

then the for loop (for name in f_list) --> goes through each csv.. for each csv it reads it in as pandas df
                                       --> for each df it calls process 

process(df) --> this is the function where u should add code for a single ETF. the etf's metrics are in the df. 




   1) Technical Indicators on ETF's (50vs200 Exponentional Moving Averages, MACD vs MACD Signal, Relative Strength Index (RSI))
   2) Technical Indicators on stocks in sector (50vs200 Exponentional Moving Averages, MACD vs MACD Signal, Relative Strength Index)
        - do all the scoring, and rank the stocks for each sector 
        - look at neural nets and see how to properly incorporate weighted metric inputs 
        - Top 5 stocks for etfs that are in (buy) mode , 2 stocks for etfs that are in (sell) mode 
        - outputs a csv that indicates which stocks to buy and sell for the day 

   3) For each stock -- 
        1) PEG Ratio lower than mean --used
        2) Current Price
        3) Sharpe Ratio (make sure its high) --used
        4) Beta	
        5) Forward P/E	--used
        6) Trailing P/E	
        7) Market Cap	--used
        8) Trailing EPS	
        9) Forward EPS	--used
        10) PEG Ratio	--used
        11) Price To Book	--used
        12) E/V to EBITDA	--used
        13) Free Cash Flow	--used
        14) Deb To Equity	--used
        15) Earnings Growth	
        16) Ebitda margins	
        17) Quick Ratio	
        18) Target Mean Price	
        19) Return on Equity  --used 	
        20) Revenue Growth	--used
        21) Current Ratio	
        22) Dividend Yield



Things to Look at: 
  -- different modules to scrape market data 
  -- understand options/futures trading more 


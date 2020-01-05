# forecasting-econometric-time-series-with-genetic-dynamic-bayesian-networks-includes-data-and-softwar
Please use all 5 macro-economic data.frames with 244 to 263 time series going back to 01-01-1991. 
The data.frames are: gdpDb( gross domestic product ); cpiDb ( consumer price index ), payemsDb ( payroll employment ), unrateDb ( unemployment rate ). I also included stockDb, which contains most of the SP500. 
These are all tab delimited text files with clear concise column names. Dates serve as row.names for the data.frame. 
Check out the vignette (with the programs folded into the R notebook) results are in html format.
Software includes an integer valued Genetic Algorithm which samples from the lagged data.frame (the dynamic data.frame) derived from cpiDb in this case study.
I have provided you with the intermediate results from the genetic algorithm, there is one result for each macro-economic indicator: df.bn.cpi; df.bn.gdp; df.bn.unrate; df.bn.payems.
Otherwise, you must create your own population.
After creating an initial population running the function corrConn (correlation network connectivity) Mutate and crossOver will operate on this matrix, each producing new samples and corresponding fitness scores and measures. Rank the merged matrix selecting the fittest 5-10%.
Run the function GeneFreq to see which time series most frequently appeared in successful networks.
Run the function showStrength on the best 20 dyanmic bayesian networks. 


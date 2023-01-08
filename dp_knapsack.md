- 2d array $dp[j][i]$, select item from $[0, ..., i]$ put in knapsack of size $j$.
- if doesn't put item i in knapsack j: $dp[i-1][j]$
- if put item i in knapsack j: $dp[i-1][j-w_i] + value[i]$ max value without i, 
- induction function: $dp[i][j] max(dp[i-1][j], dp[i-1][j-w_i] + value[i]), max of with or without i. 


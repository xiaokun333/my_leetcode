2d array dp[j][i], select item from [0, ..., i] put in knapsack of size j.
if doesn't put item i in knapsack j: dp[i-1][j]
if put item i in knapsack j: dp[i-1][j-w_i]

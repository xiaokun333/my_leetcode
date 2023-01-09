## 01 knapsack
- 2d array $dp[j][i]$, select item from $[0, ..., i]$ put in knapsack of size $j$.
- if doesn't put item i in knapsack j: $dp[i-1][j]$
- if put item i in knapsack j: $dp[i-1][j-w_i] + value[i]$ max value without i, 
- **Number of ways**: induction function: $dp[i][j] max(dp[i-1][j], dp[i-1][j-w_i] + value[i])$, max of with or without i. 
- 倒叙遍历 j，iterate reverse j (knapsack), adding every item once
- **Number of combinations**: dp[j] += dp[j-nums[i]] i 是物品，j是背包，先遍历物品，再遍历背包

##knapsack w/o repitition
- 正序遍历 j, iterate j (knapsack) small to large, each item used multiple times
- for (j = weight(), j M 

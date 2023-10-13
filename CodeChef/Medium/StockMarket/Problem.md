## Problem Statement

Chef has started learning about the stock market and has already selected a favorite stock. He traded the stock for N consecutive days. Let Ai denote the profit earned by Chef on the ith day. Note that Ai < 0 indicates that Chef had a loss on the ith day.

Chef wants to find the maximum amount of profit he would have earned if he skipped trading for exactly one day.

### Input Format

The first line of input will contain a single integer T, denoting the number of test cases.

Each test case consists of multiple lines of input.

The first line of each test case contains N — the number of days.

The next line denotes N space-separated integers, denoting the profit earned by Chef on the ith day.

### Output Format

For each test case, output on a new line the maximum amount of profit Chef would have earned if he skipped trading for exactly one day.

### Constraints

- 1 ≤ T ≤ 1000
- 1 ≤ N ≤ 10^5
- -100 ≤ Ai ≤ 100
- The sum of N over all test cases won't exceed 10^6.

### Sample

Input:
```
4
3
1 -2 3
4
4 1 5 1
4
10 -10 -10 10
5
-5 -4 -3 -2 -1
4
10
```
Output:
```
4
10
10
-10
```
### Explanation

Test case 1: To make the maximum profit, Chef would have skipped day 2. The total profit for the rest of the days is 1 + 3 = 4.

Test case 2: To make the maximum profit, Chef would have skipped day 4. The total profit for the rest of the days is 1 + 4 + 5 = 10.

Test case 3: To make the maximum profit, Chef would have skipped day 3. The total profit for the rest of the days is 10 - 10 + 10 = 10.

Test case 4: To make the maximum profit, Chef would have skipped day 1. The total profit for the rest of the days is -4 - 3 - 2 - 1 = -10.

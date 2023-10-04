# PROBLEM STATEMENT

There are three cards with letters 𝚊 , 𝚋 , 𝚌 placed in a row in some order. You can do the following operation at most once:
Pick two cards, and swap them.

Is it possible that the row becomes 𝚊𝚋𝚌 after the operation? Output "YES" if it is possible, and "NO" otherwise.

### INPUT FORMAT

The first line contains a single integer t (1 ≤ t ≤ 6) — the number of test cases. The only line of each test case contains a single string consisting of each of the three characters 𝚊 , 𝚋 , and 𝚌 exactly once, representing the cards.

### OUTPUT FORMAT

For each test case, output "YES" if you can make the row 𝚊𝚋𝚌 with at most one operation, or "NO" otherwise.

### SAMPLE 1:

| INPUT | OUTPUT |
| -------- | -------- |
| 6 |  |
| abc | YES |
| acb | YES |
| bac | YES |
| bca | NO |
| cab | NO |
| cba | NO |


#### Explanation:

In the first test case, we don't need to do any operations, since the row is already 𝚊𝚋𝚌
In the second test case, we can swap 𝚌 and 𝚋 : 𝚊𝚌𝚋→𝚊𝚋𝚌
In the third test case, we can swap 𝚋 and 𝚊 : 𝚋𝚊𝚌→𝚊𝚋𝚌
In the fourth test case, it is impossible to make 𝚊𝚋𝚌 using at most one operation.


## Problem Statement

Chef has started a new job as an insurance agent. Each insurance costs X dollars, and Chef gets a 20% commission on selling each insurance. Find the minimum number of insurances Chef needs to sell to earn at least 100 dollars.

### Input Format

The first line of input will contain a single integer T, denoting the number of test cases.

Each test case consists of a single integer X, the cost of an insurance.

### Output Format

For each test case, output on a new line the minimum number of insurances Chef needs to sell to earn at least 100 dollars.

### Constraints

- 1 ≤ T ≤ 100
- 1 ≤ X ≤ 100

### Sample

Input:
```
4
20
80
1
5
25
```
Output:
```
25
7
500
100
```

### Explanation

Test case 1: On selling 1 insurance, Chef earns 20% of 20, which is 4 dollars. This means that Chef needs to sell 25 insurances to earn 100 dollars.

Test case 2: On selling 1 insurance, Chef earns 20% of 80, which is 16 dollars. On selling 6 insurances, Chef will earn 96 dollars. Thus, he would need to sell a minimum of 7 insurances to earn at least 100 dollars.

Test case 3: On selling 1 insurance, Chef earns 20% of 1, which is 0.2 dollars. This means that Chef needs to sell 500 insurances to earn 100 dollars.

Test case 4: On selling 1 insurance, Chef earns 20% of 5, which is 1 dollar. This means that Chef needs to sell 100 insurances to earn 100 dollars.

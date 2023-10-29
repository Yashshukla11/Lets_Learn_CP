# Problem
A. Short Substrings
time limit per test2 seconds
memory limit per test256 megabytes
inputstandard input
outputstandard output
Alice guesses the strings that Bob made for her.

At first, Bob came up with the secret string a
 consisting of lowercase English letters. The string a
 has a length of 2
 or more characters. Then, from string a
 he builds a new string b
 and offers Alice the string b
 so that she can guess the string a
.

Bob builds b
 from a
 as follows: he writes all the substrings of length 2
 of the string a
 in the order from left to right, and then joins them in the same order into the string b
.

For example, if Bob came up with the string a
="abac", then all the substrings of length 2
 of the string a
 are: "ab", "ba", "ac". Therefore, the string b
="abbaac".

You are given the string b
. Help Alice to guess the string a
 that Bob came up with. It is guaranteed that b
 was built according to the algorithm given above. It can be proved that the answer to the problem is unique.

### Input
The first line contains integer n (1 ≤ n ≤ 5000) — the number of children in the school. The second line contains n integers t1, t2, ..., tn (1 ≤ ti ≤ 3), where ti describes the skill of the i-th child.
### Output
In the first line output integer w — the largest possible number of teams.

Then print w lines, containing three numbers in each line. Each triple represents the indexes of the children forming the team. You can print both the teams, and the numbers in the triplets in any order. The children are numbered from 1 to n in the order of their appearance in the input. Each child must participate in no more than one team. If there are several solutions, print any of them.

If no teams can be compiled, print the only line with value w equal to 0.

### Sample input outputs

### Examples
input
7
1 3 1 3 2 1 2
output
2
3 5 2
6 7 4
input
4
2 1 1 2
output
0
# Problem Statement
You are given a string `s` consisting of lowercase English letters. The task is to perform a duplicate removal operation, which involves choosing two adjacent and equal letters and removing them from the string. This operation is repeated until it can no longer be performed.

Return the final string after all such duplicate removals have been made. It can be proven that the answer is unique.

# Examples

**Example 1:**
```
Input: s = "abbaca"
Output: "ca"
Explanation: 
For example, in "abbaca" we could remove "bb" since the letters are adjacent and equal, and this is the only possible move. The result of this move is that the string is "aaca", of which only "aa" is possible, so the final string is "ca".
```

**Example 2:**
```
Input: s = "azxxzy"
Output: "ay"
```

# Constraints
- 1 <= s.length <= 105
- `s` consists of lowercase English letters.

---

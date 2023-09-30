# PROBLEM STATEMENT

Given an array of bird sightings where every element represents a bird type id, determine the id of the most frequently sighted type. If more than 1 type has been spotted that maximum amount, return the smallest of their ids.
Example
arr=[1,1,2,2,3]
There are two each of types 1 and 2 , and one sighting of type 3 . Pick the lower of the two types seen twice: type 1.

### INPUT FORMATE

The first line contains an integer,n, the size of arr. The second line describes arr as n space-separated integers, each a type number of the bird sighted.

### CONSTRAINTS

5 ≤ n ≤ 2 x 10^5
It is guaranteed that each type is 1 , 2 , 3 , 4 or 5.

### SAMPLE 1:

| INPUT | OUTPUT |
| -------- | -------- |
| 11 |  |
| 1 2 3 4 5 4 3 2 1 3 4 | 3 |

#### Explanation:
The different types of birds occur in the following frequencies:

Type 1: 2<br>
Type 2: 2<br>
Type 3: 3<br>
Type 4: 3<br>
Type 5: 1<br>
Two types have a frequency of 3, and the lower of those is type 3.

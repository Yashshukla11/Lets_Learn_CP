## SOLUTION :
Here is the CPP code for the problem.

```cpp
class Solution {
public:
    bool searchMatrix(vector<vector<int>>& matrix, int target) {
        int rows=matrix.size()-1,cols=matrix[0].size()-1;
        int rowi=0,coli=cols;
        while(rowi<=rows&&coli>=0){
            int element=matrix[rowi][coli];
            if(element==target){
                return true;
            }
            else if(element>target){
                coli--;
            }
            else{
                rowi++;
            }
        }
        return false;
    }
};
```
Hope it helps.

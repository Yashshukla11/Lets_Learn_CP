## SOLUTION
Here is the CPP code for the problem.

```cpp

class Solution {
public:
    string removeDuplicates(string s) {
        m:
        if(s.size()>=2){
        
        for(int i=0;i<s.length()-1;i++){
            if(s[i]==s[i+1]){
                s.erase(i,2);
                goto m;
            }
        }
        }
        
            return s;
    }
};


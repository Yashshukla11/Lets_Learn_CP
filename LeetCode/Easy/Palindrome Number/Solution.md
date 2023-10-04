Here's the cpp solution:

```cpp
class Solution {
public:
    bool isPalindrome(int x) {
        long long int rev=0,temp=x;
        if(x<0){
            return false;
        }
        else{
            while(temp!=0){
            rev=rev+(temp%10);
            rev=rev*10;
            temp=temp/10;
            }
            rev=rev/10;
            if(rev==x)
            return true;
            return false;
        }
    }
};
```
Hope it helps.
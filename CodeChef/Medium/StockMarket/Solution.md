```cpp
#include <iostream>
using namespace std;

int main() {
    int t;
    cin>>t;
    while(t--){
        int n,x=101,sum=0;
        cin>>n;
        int arr[n];
        for(int i=0;i<n;i++){
            cin>>arr[i];
            if(arr[i]<x){
                x=arr[i];
            }
            sum=sum+arr[i];
        }
        cout<<sum-x<<endl;
    }
	

	return 0;
}
```

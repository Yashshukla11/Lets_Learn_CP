Here is the solution of the problem

```cpp
#include<iostream>
using namespace std;
int main(){
    long long int t;
    cin>>t;
    while (t--){
        long long int n,u,d,count=0,s=1;
        cin>>n>>u>>d;
        long long int arr[n];
        for(long long int i=0;i<n;i++){
            cin>>arr[i];
        }
        for(long long int i=0;i<n-1;i++){
            if(arr[i]==arr[i+1]){
                s++;
            }
            
            
            if(arr[i]<arr[i+1]){
                if(arr[i+1]-arr[i]<=u){
                    s=s+1;
                }
                else{
                    break;
                }
            }
            if(arr[i]>arr[i+1]){
                if(count==0){
                    if(arr[i+1]-arr[i]<=d){
                    s=s+1;
                }
                    else if(arr[i+1]-arr[i]>d){
                    s=s+1;
                    count=count+1;
                }
                }
                if(count>=1){
                if(arr[i+1]-arr[i]<=d){
                    s=s+1;
                }
                else{
                    break;
                }
                }
            }
        }
        cout<<s<<endl;
    }
    return 0;
}

```

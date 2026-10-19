Code Lucky sum of digits;
```cpp
#include<bits/stdc++.h>
using namespace std;
bool fun(int n,vector<int>&ans){
    if(n==0) return true;
    if(n<0) return false;
    else{
        if(fun(n-7,ans)==true){
            ans.push_back(7);
            return true;
        }
        if(fun(n-4,ans)==true){
            ans.push_back(4);
            return true;
        }
        return false;
    }
}
int main(){
    int n;
    cin>>n;
    vector<int> ans;
    if(fun(n,ans)){
        sort(ans.begin(),ans.end());
        for(auto i :ans){
            cout<<i;
        }
        return 0;
        
    }
    cout<< -1;
}
```
<img width="914" height="467" alt="image" src="https://github.com/user-attachments/assets/c03431e4-744f-4f1b-8f4d-06424c7d294c" />

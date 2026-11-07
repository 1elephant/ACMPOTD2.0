CODE: Fancy Fence
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int t;
    cin>>t;
    vector<int>v(t);
    for(int i=0;i<t;i++){
        cin>>v[i];
    }
    for(int i=0;i<t;i++){
        if(v[i]<=0){
            cout<<"NO\n";
        }
        else if(360%(180-v[i])!=0){
            cout<<"NO\n";
        }
        else{
            cout<<"YES\n";
        }
    }
}
```
<img width="810" height="349" alt="image" src="https://github.com/user-attachments/assets/6bda9e43-a29b-400d-b144-e09294af16cf" />

CODE : Yaroslav and Permutations
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> v(n);
    map<int,int> f;
    int mx=0;
    for(int i=0;i<n;i++){
        cin>>v[i];
        f[v[i]]++;
        mx=max(mx,f[v[i]]);
    }
    if(mx<=(n+1)/2){
        cout<<"YES";
    }
    else{
        cout<<"NO";
    }
}
```
<img width="823" height="328" alt="image" src="https://github.com/user-attachments/assets/a421810c-d8d9-4900-b793-db6f7a06dd7d" />

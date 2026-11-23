CODE : Extra-terrestrial Intelligence
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> v;
    char c;
    for(int i=0;i<n;i++){
        cin>>c;
        if(c=='1') v.push_back(i);
    }
    int d=v[1]-v[0];
    for(int i=2;i<v.size();i++){
        if(v[i]-v[i-1]!=d){
            cout<<"NO\n";
            return 0;
        }
    }
    cout<<"YES\n";
    return 0;
}

```
<img width="767" height="416" alt="image" src="https://github.com/user-attachments/assets/96f5b504-01bb-438f-a080-b4aed7f6c0e8" />

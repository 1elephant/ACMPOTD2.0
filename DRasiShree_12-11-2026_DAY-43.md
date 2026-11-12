CODE : Hexadecimal's Numbers
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    long long n;
    cin>>n;
    queue<long long>q;
    q.push(1);
    int ans=0;
    while(!q.empty()){
        long long x=q.front();
        q.pop();
        if(x>n) continue;
        ans++;
        if(x*10<=n)
            q.push(x*10);
        if(x*10+1<=n)
            q.push(x*10+1);
    }
    cout<<ans;
}
```
<img width="883" height="361" alt="image" src="https://github.com/user-attachments/assets/bf4ccb3f-b7dd-42ac-9250-19637e8d2b50" />

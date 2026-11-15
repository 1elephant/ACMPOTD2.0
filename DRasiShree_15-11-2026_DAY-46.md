CODE : Next Test
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> a(n);
    for(int i=0;i<n;i++){
        cin>>a[i];
    }
    sort(a.begin(),a.end());
    int ans=1;
    for(int i=0;i<n;i++){
        if(a[i]==ans){
            ans++;
        }
    }
    cout<<ans;
}
```
<img width="897" height="358" alt="image" src="https://github.com/user-attachments/assets/cdcb98b1-2fb8-4a99-a6a2-d39bd5793e2e" />

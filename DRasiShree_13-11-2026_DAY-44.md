CODE : Strip
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> pre(n);
    int sum=0;
    for(int i=0;i<n;i++){
        int x;
        cin>>x;
        sum+=x;
        pre[i]=sum;
    }
    int cnt=0;
    for(int i=0;i<n-1;i++){
        if(pre[i]==sum-pre[i]){
            cnt++;
        }
    }

    cout<<cnt;
}
```
<img width="895" height="407" alt="image" src="https://github.com/user-attachments/assets/ba1d6cd6-d019-4495-81c3-3e5355c3d7b6" />

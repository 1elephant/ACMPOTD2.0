CODE : Fortune telling
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    int a[105],sum=0,mn=INT_MAX;
    for(int i=0;i<n;i++){
        cin>>a[i];
        sum+=a[i];
        if(a[i]%2==1) mn=min(mn,a[i]);
    }
    if(sum%2==0){
        if(mn!=INT_MAX) sum-=mn;
        else sum=0;
    }
    cout<<sum;
}
```
<img width="887" height="330" alt="image" src="https://github.com/user-attachments/assets/701d98b1-bbf2-4aa4-bef9-8308b7f0e4d8" />

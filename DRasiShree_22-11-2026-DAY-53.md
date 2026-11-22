CODE : IQ Test
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n,a[100],even=0,odd=0,ei,oi;
    cin>>n;
    for(int i=0;i<n;i++){
        cin>>a[i];
        if(a[i]%2==0){
            even++;
            ei=i+1;
        }
        else{
            odd++;
            oi=i+1;
        }
    }
    if(even==1) cout<<ei;
    else cout<<oi;
    return 0;
}
```
<img width="886" height="362" alt="image" src="https://github.com/user-attachments/assets/7e44cb91-f5fe-43fb-b2e1-282310d041c0" />

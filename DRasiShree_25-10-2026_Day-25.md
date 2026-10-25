CODE : CANDY BAG
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    for(int i=0;i<n;i++){
        for(int j=0;j<n/2;j++){
            int x=i*(n/2) +j+1;
            cout<<x<<" "<<n*n+1-x<<" ";
        }
        cout<<endl;
    }
}
 
```
<img width="896" height="314" alt="image" src="https://github.com/user-attachments/assets/2e4bac65-5cab-42c7-8206-587a84dcf764" />

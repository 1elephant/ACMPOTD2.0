CODE : Coin
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    while(n>1){
        cout<<n<<" ";
        int j=2;
        while(n%j!=0){
            j++;
        }
        n=n/j;
    }
    cout<<1;
}
```
<img width="890" height="312" alt="image" src="https://github.com/user-attachments/assets/275f072c-1f25-4451-8831-dba9f5922a58" />

CODE: Alice, Bob and Chocolate
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> t(n);
    for(int i=0;i<n;i++){
        cin>>t[i];
    }
    int a=0;
    int b=n-1;
    int ta=0;
    int tb=0;
    while(a<=b){
        if(ta<=tb){
            ta+=t[a];
            a++;
        }
        else{
            tb+=t[b];
            b--;
        }
    }
    cout<<a<<" "<<n-1-b;
}
```
<img width="892" height="419" alt="image" src="https://github.com/user-attachments/assets/17fe2a18-70f0-4555-8102-411e48952572" />

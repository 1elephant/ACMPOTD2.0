Chat Room code:
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s;
    cin>>s;
    string c="hello";
    int j=0;
    for(int i=0;i<s.length();i++){
        if(j<c.length() && s[i]==c[j]){
            j++;
        }
    }
    if(j==c.length()){
        cout<<"YES";
        return 0;
    }
    cout<<"NO";
}
```
<img width="885" height="391" alt="image" src="https://github.com/user-attachments/assets/2a0b13ed-84b3-4d6f-8650-820ca05d2ba4" />

String Task:
```cpp
#include<bits/stdc++.h>
using namespace std;
bool check(char a){
    if(a=='a' || a=='e' || a=='i'|| a=='o' || a=='u' || a=='y'){
        return true;
    }
    return false;
}
int main(){
    string s;
    cin>> s;
    string ans="";
    for(auto i :s){
        i=tolower(i);
        if(!check(i)){
            ans.push_back('.');
            ans.push_back(i);
        }
    }
    cout<<ans;
}
```
<img width="891" height="400" alt="image" src="https://github.com/user-attachments/assets/2c2a6ad7-bd1f-4615-947c-560cbd692aaa" />

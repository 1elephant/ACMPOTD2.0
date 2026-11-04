CODE : Comparing Strings
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s1,s2;
    cin>>s1>>s2;
    if(s1.length()!=s2.length()){
        cout<<"NO";
        return 0;
    }
    vector<int> pos;
    for(int i=0;i<s1.length();i++){
        if(s1[i]!=s2[i]){
            pos.push_back(i);
        }
    }
    if(pos.size()!=2){
        cout<<"NO";
        return 0;
    }
    if(s1[pos[0]]==s2[pos[1]] && s1[pos[1]]==s2[pos[0]]){
        cout<<"YES";
    }
    else{
        cout<<"NO";
    }
}
```
<img width="802" height="379" alt="image" src="https://github.com/user-attachments/assets/95b1db3e-0aca-4488-8173-4a2e641fc7f5" />

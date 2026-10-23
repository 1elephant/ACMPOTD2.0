CODE : K STRING
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int k;
    string s;
    cin>>k>>s;
    unordered_map<int,int> mp;
    for(int i=0;i<s.length();i++){
        mp[s[i]-'a']++;
    }
    string ans="";
    for(auto it:mp){
        if(it.second %k==0){
            for(int i=0;i<(it.second/k);i++){
                ans+=it.first+'a';
            }
        }
        else{
            cout<<-1;
            return 0;
        }
    }
    for(int i=0;i<k;i++){
        cout<<ans;
    }
}
```
<img width="893" height="428" alt="image" src="https://github.com/user-attachments/assets/e62d351b-38bb-4f5e-9bc2-b6e00cca9605" />

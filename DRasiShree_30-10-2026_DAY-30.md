CODE :LETTER
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s1,s2;
    getline(cin,s1);
    getline(cin,s2);
    vector<int> small(26,0);
    vector<int> big(26,0);
    for(auto it:s1){
        if(it==' ') continue;
        if(it>='A' && it<='Z'){
            big[it-'A']++;
        }
        else{
            small[it-'a']++;
        }
    }
    for(auto it:s2){
        if(it==' ') continue;
        if(it>='A' && it<='Z'){
            big[it-'A']--;
            if(big[it-'A']<0){
                cout<<"NO";
                return 0;
            }
        }
        else{
            small[it-'a']--;
            if(small[it-'a']<0){
                cout<<"NO";
                return 0;
            }
        }
    }
    cout<<"YES";
    return 0;
}
```
<img width="804" height="478" alt="image" src="https://github.com/user-attachments/assets/ce0409b1-63e8-4736-82e3-f34b4e4cd1ca" />

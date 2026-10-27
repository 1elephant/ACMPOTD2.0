CODE : Correct Solution ?
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    string m;
    cin>>n>>m;
    string s=to_string(n);
    sort(s.begin(),s.end());
    int i=-1;
    for(int j=0;j<s.length();j++){
        if(s[j]!='0'){
            break;
        }
        else{
            i++;
        }
    }
    if(n!=0){
        swap(s[i+1],s[0]);
    }
    if(s==m){
        cout<<"OK";
    }
    else{
        cout<<"WRONG_ANSWER";
    }
}
```
<img width="903" height="430" alt="image" src="https://github.com/user-attachments/assets/37baa842-b013-465f-bbe7-7730de855fdd" />

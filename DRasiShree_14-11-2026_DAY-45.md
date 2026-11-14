CODE : you are given a string
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s;
    cin>>s;
    int n=s.size();
    int ans=0;
    for(int i=0;i<n;i++){
        for(int j=i;j<n;j++){
            string sub=s.substr(i,j-i+1);
            for(int k=i+1;k<n;k++){
                if(s.substr(k,sub.size())==sub){
                    ans=max(ans,(int)sub.size());
                    break;
                }
            }
        }
    }
    cout<<ans;
}
```
<img width="892" height="381" alt="image" src="https://github.com/user-attachments/assets/8b47f3e3-4783-4367-bd19-ce045e257854" />

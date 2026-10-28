CODE : Fruits
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    int m;
    cin>>n>>m;
    vector<int> value;
    unordered_map<string,int> mp;
    for(int i=0;i<n;i++){
        int k;
        cin>>k;
        value.push_back(k);
    }
    for(int i=0;i<m;i++){
        string s;
        cin>>s;
        mp[s]++;
    }
    vector<int>freq;
    for(auto it:mp){
        freq.push_back(it.second);
    }
    sort(value.begin(),value.end());
    sort(freq.begin(),freq.end());
    int lcost=0;
    int mcost=0;
    int l=freq.size();
    for(int i=0;i<freq.size();i++){
        lcost+=(freq[l-i-1]*value[i]);
        mcost+=(freq[l-i-1]*value[n-1-i]);
    }
    cout<<lcost<<" "<<mcost;
    
}
```
<img width="802" height="452" alt="image" src="https://github.com/user-attachments/assets/e34ee484-61e7-4010-b96e-854e733409ea" />

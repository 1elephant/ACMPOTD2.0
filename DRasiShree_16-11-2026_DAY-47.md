CODE : Worm evolution
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int> a(n);
    vector<int> hash(1001,-1);
    for(int i=0;i<n;i++){
        cin>>a[i];
    }
    for(int i=0;i<n;i++){
        hash[a[i]]=i;
    }
    for(int i=0;i<n;i++){
        for(int j=0;j<n;j++){
            int x=a[i]-a[j];
            if(x>=1 && x<=1000 && hash[x]!=-1){
                int k=hash[x];
                if(i!=j && i!=k && j!=k){
                    cout<<i+1<<" "<<j+1<<" "<<k+1;
                    return 0;
                }
            }
        }
    }
    cout<<-1;
}
```
<img width="905" height="441" alt="image" src="https://github.com/user-attachments/assets/ad1e8260-f0a9-4d21-8c48-625da917931a" />

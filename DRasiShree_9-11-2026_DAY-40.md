CODE :ARRAY
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    vector<int>a(n),p,g;
    int z=0;
    for(int i=0;i<n;i++){
        cin>>a[i];
        if(a[i]>0) p.push_back(a[i]);
        else if(a[i]<0) g.push_back(a[i]);
        else z++;
    }
    vector<int>first,second,third;
    if(p.size()>0){
        first=g;
        second=p;
        if(g.size()%2==0){
            third.push_back(first.back());
            first.pop_back();
        }
    }
    else{
        first.push_back(g[0]);
        if(g.size()%2==0){
            third.push_back(g[1]);

            for(int i=2;i<g.size();i++){
                second.push_back(g[i]);
            }
        }
        else{
            second.push_back(g[1]);
            second.push_back(g[2]);
            for(int i=3;i<g.size();i++){
                third.push_back(g[i]);
            }
        }
    }
    for(int i=0;i<z;i++){
        third.push_back(0);
    }
    cout<<first.size()<<" ";
    for(int x:first) cout<<x<<" ";
    cout<<'\n';
    cout<<second.size()<<" ";
    for(int x:second) cout<<x<<" ";
    cout<<'\n';
    cout<<third.size()<<" ";
    for(int x:third) cout<<x<<" ";
    cout<<'\n';
}
```
<img width="899" height="382" alt="image" src="https://github.com/user-attachments/assets/6bc3c667-37ed-432d-9e2f-a6b99e14c37c" />
<img width="887" height="341" alt="image" src="https://github.com/user-attachments/assets/47b56c42-b206-47e0-8dd6-5080271827c5" />

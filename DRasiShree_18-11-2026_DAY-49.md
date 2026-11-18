CODE : coin
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s;
    pair<int,char> a[3]={{0,'A'},{0,'B'},{0,'C'}};

    for(int i=0;i<3;i++){
        cin>>s;
        int x=s[0]-'A',y=s[2]-'A';
        if(s[1]=='>') a[x].first++,a[y].first--;
        else a[y].first++,a[x].first--;
    }

    sort(a,a+3);

    if(a[0].first==a[1].first || a[1].first==a[2].first){
        cout<<"Impossible";
        return 0;
    }

    for(int i=0;i<3;i++) cout<<a[i].second;
}
```
<img width="899" height="382" alt="Screenshot 2026-11-09 140306" src="https://github.com/user-attachments/assets/2f58f787-303e-49c2-ba5e-fbb47f4ba8b7" />

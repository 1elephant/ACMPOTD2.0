CODE : CHESS
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string r,k;
    cin>>r>>k;
    int rx=r[0]-'a',ry=r[1]-'1';
    int kx=k[0]-'a',ky=k[1]-'1';
    int ans=0;
    for(int i=0;i<8;i++){
        for(int j=0;j<8;j++){
            if((i==rx && j==ry) || (i==kx && j==ky)) continue;
            if(i==rx || j==ry) continue;
            int dx=abs(i-kx);
            int dy=abs(j-ky);
            if((dx==2 && dy==1) || (dx==1 && dy==2)) continue;
            int dxr=abs(i-rx);
            int dyr=abs(j-ry);
            if((dxr==2 && dyr==1) || (dxr==1 && dyr==2)) continue;
            ans++;
        }
    }
    cout<<ans;
}
```
<img width="916" height="411" alt="image" src="https://github.com/user-attachments/assets/e14db33e-f15c-4d18-b929-94aea44fe6af" />

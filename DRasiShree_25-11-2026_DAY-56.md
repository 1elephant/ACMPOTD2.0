CODE :Square earth
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n,x1,y1,x2,y2;
    cin>>n>>x1>>y1>>x2>>y2;
    int p1,p2;
    if(y1==0) p1=x1;
    else if(x1==n) p1=n+y1;
    else if(y1==n) p1=3*n-x1;
    else p1=4*n-y1;
    if(y2==0) p2=x2;
    else if(x2==n) p2=n+y2;
    else if(y2==n) p2=3*n-x2;
    else p2=4*n-y2;
    int d=abs(p1-p2);
    cout<<min(d,4*n-d)<<endl;
    return 0;
}
```
<img width="896" height="346" alt="image" src="https://github.com/user-attachments/assets/0736d489-6020-40a9-adb2-98b25d079e85" />

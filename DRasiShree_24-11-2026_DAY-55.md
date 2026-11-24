CODE: FIND COLOR
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int x,y;
    cin>>x>>y;
    int s=x*x+y*y;
    int r=sqrt(s);
    if(r*r==s || x==0 || y==0){
        cout<<"black";
    }
    else{
        r++;
        if((r%2==1 && x*y>0) || (r%2==0 && x*y<0))
            cout<<"black";
        else
            cout<<"white";
    }
}
```
<img width="887" height="380" alt="image" src="https://github.com/user-attachments/assets/b76ae78f-926f-4578-9d71-85c2f5d5950e" />

CODE :parallelepiped
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int a,b,c;
    cin>>a>>b>>c;
    int x,y,z;
    x=(a*b)/c;
    y=(b*c)/a;
    z=(c*a)/b;
    int sum=4*(sqrt(x)+sqrt(y)+sqrt(z));
    cout<<sum;
}
```
<img width="806" height="249" alt="image" src="https://github.com/user-attachments/assets/732b670b-f3d7-424e-9211-51ee699cee9b" />

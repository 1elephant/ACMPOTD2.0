CODE : Double cola
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    long long n;
    cin>>n;
    long long k=1;
    while(n>5*k){
        n=n-5*k;
        k=k*2;
    }
    int index=(n-1)/k;
    vector<string> names={
        "Sheldon",
        "Leonard",
        "Penny",
        "Rajesh",
        "Howard"
    };
    cout<<names[index];
}
 
```
<img width="803" height="341" alt="image" src="https://github.com/user-attachments/assets/05e7dfd9-8acf-42eb-ae2d-60219a043582" />

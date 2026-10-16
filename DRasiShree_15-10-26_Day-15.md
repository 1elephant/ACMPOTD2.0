Football code:
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    int a=0;
    int b=0;
    string name1="";
    string name2="";
    for(int i=0;i<n;i++){
        string s;
        cin>>s;
        if(name1=="" || s==name1){
            name1=s;
            a++;
        }
        else if(name2=="" || s==name2){
            name2=s;
            b++;
        }
    }
    if(a>b){
        cout<<name1;
        return 0;
    }
    cout<< name2;
}
```
<img width="911" height="475" alt="image" src="https://github.com/user-attachments/assets/ed6eab23-9b9e-4ca8-b529-31d02510879a" />

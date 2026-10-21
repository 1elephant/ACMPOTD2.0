Code : Elevator
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    freopen("input.txt", "r", stdin);
    freopen("output.txt", "w", stdout);
    string side;
    int rail;
    cin >> side >> rail;
    if(side == "front"){
        if(rail == 1){
            cout << "L";
        }
        else{
            cout << "R";
        }
    }
    else{
        if(rail == 1){
            cout << "R";
        }
        else{
            cout << "L";
        }
    }
    return 0;
}
```
<img width="888" height="425" alt="image" src="https://github.com/user-attachments/assets/a24f376a-4ccc-4a14-a885-ff135de16d63" />

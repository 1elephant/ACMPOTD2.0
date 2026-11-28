CODE :Friends
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int m;
    cin>>m;
    vector<vector<int>> mat(6,vector<int>(6,0));
    for(int i=0;i<m;i++){
        int u,v;
        cin>>u>>v;
        mat[u][v]=1;
        mat[v][u]=1;
    }

    for(int i=1;i<=5;i++){
        for(int j=i+1;j<=5;j++){
            for(int k=j+1;k<=5;k++){
                if((mat[i][j] && mat[j][k] && mat[i][k]) ||
                   (!mat[i][j] && !mat[j][k] && !mat[i][k])){
                    cout<<"WIN";
                    return 0;
                }
            }
        }
    }

    cout<<"FAIL";
}
```
<img width="890" height="443" alt="image" src="https://github.com/user-attachments/assets/0da4edba-019c-4067-a0a9-b9e19152fdd9" />

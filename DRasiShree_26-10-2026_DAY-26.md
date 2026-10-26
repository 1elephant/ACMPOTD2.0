CODE : President's Office
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n, m;
    char r;
    cin >> n >> m >> r;
    unordered_map<char,int> mp;
    vector<vector<char>> v(n, vector<char>(m, '.'));
    for(int i=0; i<n; i++){
        for(int j=0; j<m; j++){
            cin >> v[i][j];
        }
    }
    for(int i=0; i<n; i++){
        for(int j=0; j<m; j++){
            if(v[i][j] == r){
                if(i>0 && v[i-1][j]!=r && v[i-1][j]!='.'){
                    mp[v[i-1][j]]++;
                }
                if(i<n-1 && v[i+1][j]!=r && v[i+1][j]!='.'){
                    mp[v[i+1][j]]++;
                }
                if(j>0 && v[i][j-1]!=r && v[i][j-1]!='.'){
                    mp[v[i][j-1]]++;
                }
                if(j<m-1 && v[i][j+1]!=r && v[i][j+1]!='.'){
                    mp[v[i][j+1]]++;
                }
            }
        }
    }
    cout << mp.size();
}
```
<img width="803" height="437" alt="image" src="https://github.com/user-attachments/assets/22b4ad38-323a-4bed-9f47-713d5bc444a1" />

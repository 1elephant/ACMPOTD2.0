HARD CODE : Bargaining Table
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n,m;
    cin>>n>>m;
    vector<string> mat(n);
    for(int i=0;i<n;i++){
        cin>>mat[i];
    }
    int ans=0;
    for(int r1=0;r1<n;r1++){
        for(int r2=r1;r2<n;r2++){
            int maxw=0;
            int w=0;
            for(int c=0;c<m;c++){
                bool valid=true;
                for(int k=r1;k<=r2;k++){
                    if(mat[k][c]!='0'){
                        valid=false;
                        break;
                    }
                }
                if(valid){
                    w++;
                    maxw=max(maxw,w);
                }
                else{
                    w=0;
                }
            }
            if(maxw>0){
                int h=r2-r1+1;
                ans=max(ans,2*(h+maxw));
            }
        }
    }
    cout<<ans;
}
```
<img width="803" height="465" alt="image" src="https://github.com/user-attachments/assets/df105824-7b11-4cda-a836-69d533945a01" />

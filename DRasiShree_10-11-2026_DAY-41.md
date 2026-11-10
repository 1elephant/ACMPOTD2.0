CODE :Centre Alignment
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    string s;
    vector<string>text;
    int maxlen=0;
    while(getline(cin,s)){
        text.push_back(s);
        maxlen=max(maxlen,(int)s.length());
    }
    for(int i=0;i<maxlen+2;i++){
        cout<<"*";
    }
    cout<<endl;
    bool left=true;
    for(int i=0;i<text.size();i++){
        int l=text[i].length();
        int diff=maxlen-l;
        int h=diff/2;
        if(diff%2==1){
            if(!left){
                h++;
            }
            left=!left;
        }
        cout<<"*";
        for(int j=0;j<h;j++){
            cout<<" ";
        }
        cout<<text[i];
        for(int j=0;j<diff-h;j++){
            cout<<" ";
        }
        cout<<"*"<<endl;
    }
    for(int i=0;i<maxlen+2;i++){
        cout<<"*";
    }
    cout<<endl;
}
```
<img width="849" height="467" alt="Screenshot 2026-11-10 075025" src="https://github.com/user-attachments/assets/8b30cdef-dcac-4859-a81c-9b66b98c2747" />

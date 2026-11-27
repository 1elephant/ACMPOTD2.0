CODE : Factorial
code in cpp
```cpp
#include<bits/stdc++.h>
using namespace std;
int main(){
    int n;
    cin>>n;
    int fact=1;
    for(int i=2;i<=n;i++){
        fact*=i;
    }
    cout<< fact;
} 
```
in question code asked in TCl
set n [gets stdin]
set fact 1

for {set i 2} {$i <= $n} {incr i} {
    set fact [expr {$fact * $i}]
}

puts $fact
<img width="883" height="236" alt="image" src="https://github.com/user-attachments/assets/d8649824-51a4-4cc6-a0f8-704983617ad9" />

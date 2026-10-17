YOUNG PHYSICIST

```cpp
#include <bits/stdc++.h>
using namespace std;
int main() {
    int n;
    cin >> n;
    int x = 0;
    int y = 0;
    int z = 0;
    for (int i = 0; i < n; i++) {
        int a, b, c;
        cin >> a >> b >> c;
        x += a;
        y += b;
        z += c;
    }
    if (x == 0 && y == 0 && z == 0)
        cout << "YES";
    else
        cout << "NO";
    return 0;
}
```
<img width="887" height="404" alt="image" src="https://github.com/user-attachments/assets/ef9b2ee5-92a5-486a-8e6a-7592d71a36b8" />

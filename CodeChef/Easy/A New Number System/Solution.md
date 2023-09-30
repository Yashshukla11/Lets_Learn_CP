## SOLUTION :
Here is the CPP code for the problem.

```cpp
#include <iostream>

using namespace std;

// Function to check if it's possible to create a grid with X good cells
string is_possible(int N, int X) {
    if (X == 1 || X == N || X == 2 * N) {
        return "Yes";
    }
    return "No";
}

int main() {
    int T;
    cin >> T;

    // Process each test case
    for (int i = 0; i < T; i++) {
        int N, X;
        cin >> N >> X;
        string result = is_possible(N, X);
        cout << result << endl;
    }

    return 0;
}


```
Hope it helps. 😀

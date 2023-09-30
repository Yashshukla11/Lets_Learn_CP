## SOLUTION :
Here is the CPP code for the problem.

```cpp
#include <iostream>
#include <vector>
#include <unordered_map>

using namespace std;

int migratoryBirds(vector<int> arr) {
    unordered_map<int, int> birdCount; // Hash map to store bird type counts
    
    // Count the occurrences of each bird type
    for (int bird : arr) {
        if (birdCount.find(bird) != birdCount.end()) {
            birdCount[bird]++;
        } else {
            birdCount[bird] = 1;
        }
    }

    // Find the bird type(s) with the highest count
    int maxCount = 0;
    vector<int> mostFrequentBirds;
    
    for (const auto& entry : birdCount) {
        if (entry.second > maxCount) {
            maxCount = entry.second;
            mostFrequentBirds.clear();
            mostFrequentBirds.push_back(entry.first);
        } else if (entry.second == maxCount) {
            mostFrequentBirds.push_back(entry.first);
        }
    }

    // Find the lowest id among the most frequent birds
    int lowestId = mostFrequentBirds[0];
    for (int bird : mostFrequentBirds) {
        if (bird < lowestId) {
            lowestId = bird;
        }
    }

    return lowestId;
}

int main() {
    int n;
    cin >> n;
    vector<int> arr(n);

    for (int i = 0; i < n; i++) {
        cin >> arr[i];
    }

    int result = migratoryBirds(arr);
    cout << result << endl;

    return 0;
}

```
Hope it helps. 😀

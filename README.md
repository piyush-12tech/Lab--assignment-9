#include <iostream>
#include <queue>
using namespace std;

int main() {
    priority_queue<int> maxH;
    priority_queue<int, vector<int>, greater<int>> minH;

    int a[] = {40, 10, 30, 20, 50};

    for (int x : a) {
        maxH.push(x);
        minH.push(x);
    }

    cout << "Max Heap: ";
    while (!maxH.empty()) {
        cout << maxH.top() << " ";
        maxH.pop();
    }

    cout << "\nMin Heap: ";
    while (!minH.empty()) {
        cout << minH.top() << " ";
        minH.pop();
    }
}

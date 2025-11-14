# C++ Array Practice Solutions

## 1. Store 5 integers and find sum
```cpp
#include <iostream>
using namespace std;

int main() {
    int arr[5], sum = 0;

    cout << "Enter 5 integers:\n";
    for(int i = 0; i < 5; i++) {
        cin >> arr[i];
        sum += arr[i];
    }

    cout << "Sum = " << sum;
    return 0;
}
```

### Output
```
Enter 5 integers:
10
20
30
40
50
Sum = 150
```

---

## 2. Character array reverse
```cpp
#include <iostream>
using namespace std;

int main() {
    char arr[5];

    cout << "Enter 5 characters:\n";
    for(int i = 0; i < 5; i++)
        cin >> arr[i];

    cout << "Reversed: ";
    for(int i = 4; i >= 0; i--)
        cout << arr[i] << " ";

    return 0;
}
```

### Output
```
Enter 5 characters:
a b c d e
Reversed: e d c b a
```

---

## 3. Highest marks
```cpp
#include <iostream>
using namespace std;

int main() {
    int marks[5], highest = 0;

    cout << "Enter marks of 5 students:\n";
    for(int i = 0; i < 5; i++) {
        cin >> marks[i];
        if(marks[i] > highest)
            highest = marks[i];
    }

    cout << "Highest Mark = " << highest;
    return 0;
}
```

### Output
```
Enter marks of 5 students:
70
80
75
65
90
Highest Mark = 90
```

---

## 4. Dynamic array largest element
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter size: ";
    cin >> n;

    int *arr = new int[n];
    cout << "Enter " << n << " numbers:\n";

    int largest = -1e9;
    for(int i = 0; i < n; i++) {
        cin >> arr[i];
        if(arr[i] > largest)
            largest = arr[i];
    }

    cout << "Largest = " << largest;

    delete[] arr;
    return 0;
}
```

### Output
```
Enter size: 5
Enter 5 numbers:
5
10
20
15
7
Largest = 20
```

---

## 5. Dynamic array average
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter size: ";
    cin >> n;

    int *arr = new int[n];
    cout << "Enter " << n << " numbers:\n";

    double sum = 0;
    for(int i = 0; i < n; i++) {
        cin >> arr[i];
        sum += arr[i];
    }

    cout << "Average = " << sum / n;

    delete[] arr;
    return 0;
}
```

### Output
```
Enter size: 5
Enter 5 numbers:
10
20
30
40
50
Average = 30
```

---

## 6. Dynamic array of names
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "How many names? ";
    cin >> n;

    char **names = new char*[n];

    for(int i = 0; i < n; i++) {
        names[i] = new char[50];
        cout << "Enter name " << i + 1 << ": ";
        cin >> names[i];
    }

    cout << "\nNames entered:\n";
    for(int i = 0; i < n; i++)
        cout << names[i] << endl;

    for(int i = 0; i < n; i++)
        delete[] names[i];

    delete[] names;

    return 0;
}
```

### Output
```
How many names? 3
Enter name 1: Ali
Enter name 2: Sara
Enter name 3: Ahmed

Names entered:
Ali
Sara
Ahmed
```

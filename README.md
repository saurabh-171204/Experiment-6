# Experiment-6
# AIM
To study and implement C++ decision making statement loops.
# THEORY
## Types of Loops in C++ :
### for Loop:
Executes a block of code repeatedly until a specified condition is false.
### while Loop:
Repeats a block of code as long as a specified condition is true.
Condition: Checked before each iteration. If false, the loop terminates.
### do-while Loop:
Similar to while loop, but guarantees at least one execution of the block of code.
Condition: Checked after each iteration. If false, the loop terminates.
### Nested loops:
Nested loops involve placing one loop inside another. They can be useful for handling multi-dimensional data or performing complex iterations.
Nested loops can be quite powerful but can also lead to performance issues if not used carefully, especially with large datasets or high iteration counts.

# CODE
### 1. for loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main()
{
    int i;
    for(i=0;i<10;i++)
    {
        cout<<"heloo world("<<i+1<<")"<<endl;
    }
}
```

### 2. while loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main() 
{
    int input = 1;
    while (input <= 15) {
        std::cout << "\n" << input;
        input++;
    }
}
```

### 3. do-while loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include <iostream>

using namespace std;

int main() {
    int number = 1;
    do {
        cout << number << endl;
        number++;
    } while (number <= 10);
    return 0;
}
```

### 4. Nested for loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main() {
    for (int i = 1; i <= 1; i++) {
        for (int j = 1; j <= 10; j++) {
            std::cout << j << " ";
        }
    }
    std::cout << std::endl;
    return 0;
}
```

### 5. Nested while loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main()
{
    int i = 1;
    while (i <= 10) {
        int j = 1;
        while (j <= i) {
            std::cout << j << " ";
            j++;
        }
        std::cout << std::endl;
        i++;
    }
    return 0;
}
```

### 6. Nested do-whhile loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main() {
    int i = 1;
    do {
        int j = 1;
        do {
            std::cout << j << " ";
            j++;
        } while (j <= 10);
        i++;
    } while (i <= 1);
    std::cout << std::endl;
    return 0;
}
```

### 7. Nested for while loop:
```
//Saurabh
//23070123166
//entc B2
//experiment 6
#include<iostream>
using namespace std;
int main()
{
    int i,j,k=0,n;
    cout<<"enter number of rows-";
    cin>>n;
    for(i=1;i<=n;i++)
    {
        for(j=1;j<=(n-i);j++)
        {
            cout<<" ";
        }
        while(k!=(i-1))
        {
            cout<<"* ";
            k++;
        }
        k=0;
        cout<<endl;
    }
    cout<<endl;
}
```

# Conclusion
Loops allow repetitive execution of code. A for loop iterates over a sequence and is used when the number of iterations is known.
A while loop runs as long as a condition is true, useful for uncertain iteration counts.
Nested loops enable complex iteration, such as iterating over multi-dimensional arrays. Each type offers different control and flexibility for managing code flow.

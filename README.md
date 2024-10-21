# Experiment 16



## Aim:
To study and implement Exception Handling


## Apparatus:
Vs Code, Github


## Theory:

Exception handling in C++ is a way to handle errors or unexpected conditions during the execution of a program. This allows a program to respond to errors without crashing and provides a way handle error conditions.

In C++, exception handling is done using three primary keywords: try, throw, and catch. The program is to "try" a block of code and if an error occurs, "throw" an exception, which is then "caught" by a matching "catch" block.

### Try:
A try block encloses the code that might throw an exception. If any exception occurs within the try block, the corresponding catch block is then executed.

### Throw:
A throw expression is used to signal that an error has occured during the program’s execution.

### Catch:
A catch block is used to handle exceptions thrown by the throw expression. It defines how to handle exceptions of a particular type. You can use multiple catch blocks to handle different types of exceptions.

## Code:

### Division exception:
```
#include <iostream>
using namespace std;

int main(){
  float n1, n2, ans;
  cout<<"Enter values of numbers 1 & 2: ";
  cin>>n1>>n2;
  try{
    if(n2==0){
      throw n2;
    }
    else{
      ans=n1/n2;
      cout<<"Answer = "<<ans<<endl;
    }
  }
  catch(float num){
    cout<<"\nERROR: Division by"<<num<<endl;
  }
}
```
### Output:
<img width="1087" alt="Screenshot 2024-10-21 at 9 06 54 AM" src="https://github.com/user-attachments/assets/bde87b8f-1de8-43b9-b8ec-4b06fa69c2c3">

### Age:
```
#include<iostream>
using namespace std;

int main(){
    int age;
    cout<<"Enter age: ";
    cin>>age;
    try{
        if(age<18){
            throw age;
        }
        else{
            cout<<"Age: "<<age<<"\nAPPROVED"<<endl;
        }
    }
    catch(int a){
        cout<<"\nERROR: Underage! ("<<age<<")"<<endl;
    }
}
```
### Output:
<img width="1100" alt="Screenshot 2024-10-21 at 9 08 30 AM" src="https://github.com/user-attachments/assets/3ba00a28-8d6e-4ef7-ac11-2848bb6b3dac">


## Conclusion:
This program helps us understand how exceptional handling works in C++. The working of the different keywords like try,throw and catch are also explained in this program.

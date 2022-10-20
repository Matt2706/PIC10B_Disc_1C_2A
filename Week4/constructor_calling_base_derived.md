Constructor call order:
```
// C++ program to show the order of constructor call
// in single inheritance
  
#include <iostream>
using namespace std;
 
// base class
class Parent
{
    public:
     
    // base class constructor
    Parent()
    {
        cout << "Inside base class" << endl;
    }
};
 
// sub class
class Child : public Parent
{
    public:
     
    //sub class constructor
    Child()
    {
        cout << "Inside sub class" << endl;
    }
};
 
// main function
int main() {
      
    // creating object of sub class
    Child obj;
     
    return 0;
}
```
Output:
```
Inside base class
Inside sub class
```
Constructor call in Multiple Inheritance:
```
#include <iostream>
using namespace std;
 
// first base class
class Parent1
{  
    
    public:
     
    // first base class's Constructor   
    Parent1()
    {
        cout << "Inside first base class" << endl;
    }
};
 
// second base class
class Parent2
{
    public:
     
    // second base class's Constructor
    Parent2()
    {
        cout << "Inside second base class" << endl;
    }
};
 
// child class inherits Parent1 and Parent2
class Child : public Parent1, public Parent2
{
    public:
     
    // child class's Constructor
    Child()
    {
        cout << "Inside child class" << endl;
    }
};
 
// main function
int main() {
     
    // creating object of class Child
    Child obj1;
    return 0;
}
```
Output:
```
Inside first base class
Inside second base class
Inside child class
```
Reference Link: [geeksforgeeks](https://www.geeksforgeeks.org/order-constructor-destructor-call-c/)
# Experiment 11
# Aim:
To study and implement Classes and Objects

# Theory:
Object Oriented Programming (OOP):

Object-oriented programming is based on the concept of objects. In object-oriented programming data structures, or objects are defined, each with its own properties or attributes.
To understand OOP better, let us understand some key concepts of OOPS


Class:
A class is a collection of objects, a blueprint of objects defining the common attributes and behavior. This user-defined datatype holds its own instance variables, class variables and member functions which are accessed based on need. This can be done by creating a unique instance of that class.


Object:
A unique instance of a data structure that's defined by its class. It is an identifiable entity with a set of characteristics and behavior.


Inheritance:
The mechanism which creates classes that are built upon existing classes, in a new implementation while maintaining the same behaviors.


Encapsulation:
The mechanism which combines similar data and functions into a single unit called a class. It helps protect the data from any change.


Abstraction:
The mechanism that depends on the separation of the interface and implementation details of the program. It provides only the required details to the user, hiding the technical internal ones.


Polymorphism:
The mechanism which allows an object to be represented in various forms.


Let us understand the difference between Procedural Oriented Programming (POP) and Object Oriented Programming (OOP):



Procedural Oriented Programming (POP)	Object Oriented Programming (OOP)


-> It does not support inheritance.	It supports inheritance.

-> It is less secure	It is more secure.

-> It is a top-down approach.	Its is a bottom-up approach.

-> Program is divided into functions.	Program is divided into objects.

-> Data can move freely from function to another function within programs.	Object can move freely within member functions.

-> It does not use access modifiers.	Makes use of access modifiers like public, private and protected.


Advantages of Object Oriented Programming:


Reusability

Data Redundancy

Code Maintainance

Flexibility

Security

This is why C++ is preffered over C as OOP is very advantageous.

 # Code:

a.
```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0;
    double b = 3.0;
    double l = 4.0;
};
int main()
{
  cuboid c1;
  double vol = c1.h * c1.b * c1.l;
  cout<<"Volume "<<vol<<endl;
}
``` 

b.
```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 5.0,b = 3.0,l = 8.0;
    double volume()
    {
        double vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```

c.

```
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 20.0,b = 13.0,l = 17.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
``` 

d.

```
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 7.0,b = 8.0,l = 9.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    double v = c1.volume();
    c1.disp(v);
  
}
``` 

e.

```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h,b,l;
    void input()
    {
        cout<<"Enter the length: ";
        cin>>l;
        cout<<"Enter the breadth: ";
        cin>>b;
        cout<<"Enter the height: ";
        cin>>h;
    }
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    c1.input();
    double v = c1.volume();
    c1.disp(v);
  
}
```

# Conclusion:

→ We learnt about OOP in C++.

→ We learnt the use case of classes and objects in C++.


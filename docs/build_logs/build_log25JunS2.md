Date: 25 June 2026 (Session 2)
Duration: 3 hours 30 mins 
Goal():
To implement the hash function for the userdefined datatypes.

Problem():
For example i have a userdefined objects where i have various parameters such as 3 intergers 2 string 3 float, From these I only want 1 int 1 string and 1 float as the parameter.

For this what i tried is taking the paramenters finding its hash value and combining them to create a final 
hash value in this method all the three fields contribute in the hashvalue generation change in any of the fie.
The second alternative i tried was creating the hashcode on the basis of memory addreess but what happended in this case was if a 
object is created whenever we store two objects having same value or even when we print the same object it always give different 
address. 

Error1:
PS D:\CQ> g++ -g main.cpp -o tst
main.cpp: In function 'int main()':
main.cpp:42:57: error: no matching function for call to 'Employee::Employee(int, const char [9], Address)'
     Employee e(101, "John Doe", Address{123, "New York"});
                                                         ^
main.cpp:29:8: note: candidate: Employee::Employee()
 struct Employee
        ^~~~~~~~
main.cpp:29:8: note:   candidate expects 0 arguments, 3 provided
main.cpp:29:8: note: candidate: Employee::Employee(const Employee&)
main.cpp:29:8: note:   candidate expects 1 argument, 3 provided
main.cpp:29:8: note: candidate: Employee::Employee(Employee&&)
main.cpp:29:8: note:   candidate expects 1 argument, 3 provided

In this the arguments were not been decrated properly due to which errors were showing.

Error 2:
PS D:\CQ> g++ -g main.cpp -o tst
main.cpp: In function 'int main()':
main.cpp:46:13: error: 'unt' was not declared in this scope
     HashMap<unt,std::string>intmap;
             ^~~
main.cpp:46:28: error: template argument 1 is invalid
     HashMap<unt,std::string>intmap;
                            ^
main.cpp:46:28: error: template argument 3 is invalid
main.cpp:47:12: error: request for member 'insert' in 'intmap', which is of non-class type 'int'
     intmap.insert(1,"One");
            ^~~~~~
main.cpp:48:12: error: request for member 'insert' in 'intmap', which is of non-class type 'int'
     intmap.insert(20,"Twenty");
            ^~~~~~
The error was again declaring the int variable to unt due to which it was showing the error.

Outcome():
Implemented and worked on userdefined functions as worked on how everthing is going to work.
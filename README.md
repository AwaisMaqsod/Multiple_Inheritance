//# Multiple_Inheritance
//Oop c++ , multiple inheritance, through Constructor and destructor 
#include<iostream>
#include<string>
using namespace std;
//mulitple Inheritance
class Teacher{//Parent Class

		public:
			Teacher(){
				cout<<": Constructor Of Class Teacher :"<<endl;
			}
			~Teacher(){
			cout<<": Destructor Of Class Teacher :"<<endl;

			}
	
};
class Student{//Parent Class

		public:
			Student(){
				cout<<": Constructor Of Class Student :"<<endl;
			}
			~Student(){
			cout<<": Destructor Of Class Student :"<<endl;

			}
	
};
//Child Class
class Employee:public Teacher,public Student{

		public:
			Employee(){
				cout<<": Constructor Of Class Employee :"<<endl;
			}
			~Employee(){
			cout<<": Destructor Of Class Employee :"<<endl;

			}
	
};
int main(){
	Employee e;
	
	return 0;
} 

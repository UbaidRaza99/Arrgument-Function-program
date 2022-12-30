#include <iostream>
using namespace std;

//function with  no argument and no return value:
void even_odd()
{
	int num;
	cout<<"Input a number: "<<endl;
	cin>>num;
	if(num%2==1)
	cout<<"odd";
	else
	cout<<"even";
}

//function with no argument but return value:
string even_odd2()
{
	int num;
	string result;
	cout<<"Input a number: "<<endl;
	cin>>num;
	if(num%2==1)
	result = "odd";
	else
	result = "even";
	return result;
}

//function with argument but no return value:
void even_odd3(int num)
{
	if(num%2==1)
	cout<<"odd";
	else 
	cout<<"even";
}

//function with argument and return value:
string even_odd4(int num)
{
	if(num%2==1 || num==1)
	return "odd";
	else
	return "even";
}


int main()
{
	int choice,num,result;
	cout<<"Choose a function to use: "<<endl
	<<"1: function with no argument and no return value."<<endl
	<<"2: function with no argument but with return value."<<endl
	<<"3: function with argument but no return value."<<endl
	<<"4: function with argument and a return value."<<endl;
	cin>>choice;
	if(choice==1)
	even_odd();
	else if(choice ==2)
	cout<<even_odd2();
	else if(choice ==3)
	{
		cout<<"Enter a number: "<<endl;
		cin>>num;
		even_odd3(num);
	}
	else if(choice ==4)
	{
		cout<<"Enter a number: "<<endl;
		cin>>num;
		cout<<even_odd4(num);
	}
	else
	cout<<"Wrong input";
}

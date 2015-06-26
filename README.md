#include "C:\Users\Centios\Documents\Visual Studio 2013\Projects\std_lib_facilities.h"
#include <Windows.h> // Includes the Windows c++ library so we can use Sleep()

int main()
{	
	cout << "Enter the name of the person you want to write to\n";

	string first_name;	// Creats a string variable called "first_name" to store the person first name
	
		cin >> first_name;	// Read characters into "firstname"
	
		//first_name = "Dear " + first_name + ",";	// A really sloppy way of changing outputting "Dear "first_name," without changing the parameters of the next cout
		
		cout << "Dear " << first_name << "," << '\n';

			Sleep(2000);	// Suspends the process for defined ammount of time (in milliseconds) giving the text a delayed effect

			cout << "  Hey how are you? I'm doing fine. It's been pretty boring without you." << '\n';

			Sleep(1500);

			cout << "  With all my free time I've decided to start learning c++" << '\n';
				
			Sleep(1500);

			cout << "  I'm learning slowly but surely, I'm able to do some basic programs already!" << '\n' << '\n';

		Sleep(2000);

		cout << "Enter the name of another friend:" << '\n' << '\n';

	string friend_name;
	
		cin >> friend_name;
		cout << '\n';	// Starts a newline so there is space between the users input and the programs output
		Sleep(2000);
		cout << "  Have you seen " << friend_name << " lately?" << '\n' << '\n';

		char friend_sex = 0; // Creates a character variable to store the sex of our friend

		cout << "Please enter an (m) if the friend is male and (f) if the friend is female" << '\n' << '\n';
		cin >> friend_sex;
		
		cout << '\n';	// Starts a newline so there is space between the users input and the programs output

		if (friend_sex == 'm')	// If our friend_sex == "m" then execute the following else ignore
			cout << "  If you see " << friend_name << " Tell him to call me" << '\n';

		if (friend_sex == 'f')	// If our friend_sex == "f" then execute the following else ignore

			cout <<	"  If you see " << friend_name << " tell her to call me" << '\n';

		cout << '\n';	// Starts a newline so there is space between the users input and the programs output

		cout << "Please enter the age of the person your writing to" << '\n';

		int age;	// Creats an int variable called age to store recipients age

		cin >> age;

		cout << '\n'; // Starts a newline so there is space between the users input and the programs output

		cout <<	"  I hear you just had a birthday and your " << age << " years old." << '\n';

		if (age <= 0)	// If user inputs a value <= 0 into age then call "simple_error"
			simple_error("you're kidding me!");

		if (age >= 110)		// If user inputs a value <= 0 into age then call "simple_error"
			simple_error("you're kidding me!");


		if (age < 12)
			cout << "  Next year you will be " << age + 1 << '.';

		if (age == 17)
			cout << "  Next year you will be able to vote.";

		if (age > 70)
			cout << "  I hope you are enjoying retirement.";

		cout << '\n' << '\n';

		cout << "  Yours sincerely," << '\n' << '\n' << "  Cole";
	   
	    

				

	//keep_window_open();	// Keeps the windows open so we can see the outcome (only nessicary when no input is taken)
			
			
			cout << '\n';	// Starts a newline so that there is space between the message and the system("pause") line
			system("pause");	// A better version of "keep_window_open" that requires no character input
			
			return(0);
}

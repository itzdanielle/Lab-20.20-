# Lab-20.20-
#include <iostream>
#include <string>
using namespace std;

/*
_Prototypes for functions with parameters_
Examine the code and try running the program. Similarly to Lab 20.1, the main function is calling writeProverb before it is defined. Fix the error by adding a prototype for writeProverb.
*/

void writeProverb(int number)
{
	if (number == 1)
    cout << "Fortune favours the bold.\n";
  else
    cout << "Fortune favours the brave.\n";
  
}
int main() {
  int wordCode;

	cout << "Given the phrase:" << endl;
	cout << "Fortune favours the ___" << endl;

	cout << "Input a 1 if you want the sentence to be finished with bold" << endl;
	cout << "Input any other number for the word brave" << endl;

	cout << "Please input your choice now" << endl;
	cin >> wordCode; 
	cout << endl;

	writeProverb(wordCode);
}

//	******************************************************************************
//	writeProverb
//
//	task:	  This function prints a proverb. The function takes a number as an
//	          argument. If that number is a 1 it prints "Fortune favours the bold."
//	          Otherwise, it prints "Fortune favours the brave."
//	data in:   (integer) code for ending word of proverb
//	*****************************************************************************

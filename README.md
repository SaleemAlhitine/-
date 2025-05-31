#include <iostream> 
using namespace std; 
 
int main() { 
    char operation; 
    double num1, num2; 
 
    while (true) { // Using a while loop for repetition 
        cout << "Enter operation (+, -, *, /) or 'x' to exit: "; 
        cin >> operation; 
 
        if (operation == 'x') { 
            cout << "Program terminated." << endl; 
            break; // Exiting the loop if 'x' is entered 
        } 
 
        cout << "Enter first number: "; 
        cin >> num1; 
        cout << "Enter second number: "; 
        cin >> num2; 
 
        switch (operation) { 
            case '+': cout << "Result: " << num1 + num2 << endl;break ; 
            case '-': cout << "Result: " << num1 - num2 << endl;break ; 
            case '*': cout << "Result: " << num1 * num2 << endl;break ; 
            case '/':  
if (num2 != 0) 
cout << "Result: " << num1 / num2 << endl; 
else 
cout << "Error: Division by zero is not allowed!" << endl; 
break; 
default: 
cout << "Invalid operation, try again." << endl; 
} 
cout << "--------------------------\n"; 
} 
return 0; 
} 

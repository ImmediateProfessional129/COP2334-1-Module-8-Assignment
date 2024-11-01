# COP2334-1-Module-8-Assignment
This is a repository link of the COP2334-1 Module 8 Assignment

// This program is designed to determine if a charge from a user's credit account is deemed valid or invalid when purchasing a product.

// Include the iostream library.
#include <iostream>
using namespace std; // Using the standard namespace.

// Declare the main function.
int main() {
  int account_number; // Declare the account number variable.
  int account_numbers[] = {5658845, 4520125, 7895122, 8777541, 8451277, 1302850, 8080152, 4562555, 5552012, 5050552, 7825877, 1250255, 1005231, 6545231, 3852085, 7576651, 7881200, 4581002}; // Declare the array of account numbers.
  bool ifFound = false; // Declare the ifFound variable and initialize it to false.
  cout << "Enter a charge number from your account: "; // Prompt the user to enter a charge number from their account.
  cin >> account_number; // Get the user's input and store it in the account_number variable.
  for (int i = 0; i < 18; i++) { // Loop through the array of account numbers.
    if (account_numbers[i] == account_number) { // If the current account number in the array matches the user's input,
      ifFound = true; // set ifFound to true.
      break; // Break out of the loop.
    }
  }
  if (ifFound) { // If ifFound is true,
    cout << "The number you've entered is valid."; // print that the number is valid.
  } else { // Otherwise,
    cout << "The number you've entered is invalid."; // print that the number is invalid.
  }
  return 0; // Return 0 to indicate successful program execution.
}

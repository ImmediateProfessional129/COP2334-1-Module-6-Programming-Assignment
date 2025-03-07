# COP2334-1-Module-6-Programming-Assignment
This is a Github repository link for Lesson 6 Programming Exercise 6.1

// This program is designed to calculate the total number of days that a company's employees have not been showing up to work.

// Include the necessary libraries.
#include <iostream>
using namespace std;

// Add in the variables that will be used in the program.
int numEmployees();
int daysMissed(int);
double average(int, int);

// Define the main function.
int main() {
  int employees = numEmployees();
  int days = daysMissed(employees);
  double avg = average(employees, days);
  cout << "The average number of days missed per employee is " << avg << " days.";
}

// Define the numEmployees function.
int numEmployees() {
  int employees;
  cout << "How many employees are there in the company? ";
  cin >> employees;
  while (employees < 1);
  return employees;
}

// Define the daysMissed function.
int daysMissed(int employees) {
  int days;
  int total = 0;
  for (int i = 1; i <= employees; i++) {
    cout << "How many days did employee " << i << " miss? ";
    cin >> days;
    while (days < 0);
    total += days;
  }
  return total;
}

// Define the average function.
double average(int employees, int days) {
  return (double) days / employees;
}

# COP2664-1-Lesson-6-Programming-Exercise 6.1 Program #1
This is a Github repository link for Lesson 6 Programming Exercise 6.1 Program #1

// This program is designed to perform different calculations based on the user's input.

func performCalculation(a: Int, b: Int, operation: (Int, Int) -> Int) -> Int { // Function to perform the calculation
  return operation(a, b) // Return the result of the calculation
}
let result = performCalculation(a: 20, b: 5, operation: +) // Call the function with addition
print(result) // Print the result
let result2 = performCalculation(a: 24, b: 10, operation: -) // Call the function with subtraction
print(result2) // Print the result
let result3 = performCalculation(a: 14, b: 12, operation: *) // Call the function with multiplication
print(result3) // Print the result
let result4 = performCalculation(a: 18, b: 4, operation: /) // Call the function with division
print(result4) // Print the result

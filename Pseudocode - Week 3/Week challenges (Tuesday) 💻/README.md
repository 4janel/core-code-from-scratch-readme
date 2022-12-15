# Challenges

## 1. Simple Calculator with Switch

For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

1. Sum (+)
2. Subtract (-)
3. Multiplication (*)
4. Division (/)

The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use conditionals to identify which operations you should execute.

## 2. Multi Option Program

For this challenge you will create a program with multiple options using Switch (Segun), the options available are the following:

1. Sum two numbers
2. Print the day of the week given the day number
3. Print the length of a given text

This program must have a start menu where the user must select one of the previously described options. When the user selects each of the options, the program will perform the following:

1. Sum. The user enters two numbers and the result of the sum of both is printed
2. Print day of the week. The user enters a day of the week using numbers and the name of the day must be printed. For example, if the number 1 is entered, the program prints the text Lunes.
3. Calculate text length. The user enters a text and the length of the text should be printed. I was able to use the Pseint Longitud function to get the length.
When the user enters an incorrect option, a message should be printed saying that the option is not available.
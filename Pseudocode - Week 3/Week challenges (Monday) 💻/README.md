# Challenges

## 1. Simple Calculator

For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

1. Sum (+)
2. Subtract (-)
3. Multiplication (*)
4. Division (/)

The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use conditionals to identify which operations you should execute.

## 2. Special number

You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly

This was the code from the developer

        Algoritmo specialNumber
            Leer n
            Si n == 100 Entonces
                Imprimir 'This is a special number'
            FinSi
            Si n < 1000 Entonces
                Imprimir ''
            SiNo
                Imprimir 'Just a regular number'
            FinSi
            Si n % 10 == 0 Entonces
                Imprimir 'This number is multiple of 10'
            FinSi
        FinAlgoritmo

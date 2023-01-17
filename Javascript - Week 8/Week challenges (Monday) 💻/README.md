# Challenges

## 1. Training JS #7: if..else and ternary operator

Complete function `saleHotdogs`/`SaleHotDogs`/`sale_hotdogs`, function accepts 1 parameter:`n`, n is the number of hotdogs a customer will buy, different numbers have different prices (refer to the following table), return how much money will the customer spend to buy that number of hotdogs.

| number of hotdogs | price per unit (cents) |
| ----------------- | ---------------------- |
| n < 5             | 100                    |
| n >= 5 and n < 10 | 95                     |
| n >= 10           | 90                     |

You can use if..else or ternary operator to complete it.

## 2. Training JS #8: conditional statement--switch

Complete the function `howManydays`. It accepts 1 parameter `month`, which means the month of the year. Different months have a different number of days as shown in the table below. Return the number of days that are in `month`. There is no need for input validation: month will always be greater than 0 and less than or equal to 12.

```
+---------------+-------------+
|    month      |    days     |
+---------------+-------------+
|1,3,5,7,8,10,12|     31      |
+---------------+-------------+
|4,6,9,11       |     30      |
+---------------+-------------+
|2              |     28      |  (Do not consider the leap year)
+---------------+-------------+
```

**Tip:** Using `default` for most of the cases can reduce your work.

## 3. Basic calculator

Write a function called `calculate` that takes 3 values. The first and third values are numbers. The second value is a character. If the character is "+" , "-", "\*", or "/", the function will return the result of the corresponding mathematical function on the two numbers. If the string is not one of the specified characters, the function should return null (throw an `ArgumentException` in C#).

```javascript
calculate(2, "+", 4); //Should return 6
calculate(6, "-", 1.5); //Should return 4.5
calculate(-4, "*", 8); //Should return -32
calculate(49, "/", -7); //Should return -7
calculate(8, "m", 2); //Should return null
calculate(4, "/", 0); //should return null
```
Keep in mind, you cannot divide by zero. If an attempt to divide by zero is made, return null (throw an `ArgumentException` in C#)/(None in Python).
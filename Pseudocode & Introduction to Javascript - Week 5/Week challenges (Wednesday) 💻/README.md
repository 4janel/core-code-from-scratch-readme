# Challenges

## 1. Cashier

Create a function called "cashier" that pretends to be a panel of a bank should display the text: "select an option: a. to deposit. b. withdraw. c. go out." and have a value called balance that will return when finished and will print it on the screen, its initial value will be 1000. You must repeat the menu until you select the option 'c'

if we select 'a' it invokes another function called 'deposit' that will display a text on the screen that will say 'how much do you want to deposit:' it will add that value to the balance and end the function.

if we select 'b' it invokes another function called 'withdraw' that will display a text on the screen that will say 'how much do you want to withdraw:' it will subtract that value from the balance and end the function.

"select an option: a. to deposit. b. withdraw. c. go out."

a -->

"how much do you want to deposit:"

500 -->

"select an option: a. to deposit. b. withdraw. c. go out."

b -->

"how much do you want to withdraw:"

1400 -->

"select an option: a. to deposit. b. withdraw. c. go out."

c -->

100

## 2. Weather average

Write an algorithm that loops indefinitely until 'x' is entered which will calculate an average of the weather, note that for each value entered it should ask if it is fahrenheit or celsius, then ask for the value. add everything up and divide by the number of values ​​entered. The result must be returned in celsius, have a function that, in case fahrenheit is entered, transforms it to celsius in order to add them.
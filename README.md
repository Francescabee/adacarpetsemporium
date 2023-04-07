# Ada's Flooring Superstore

Click the Open Preview button above for a more readable view of these instructions.

>Candidates receiving this challenge may elect to work through live coding a solution during their interview time, or may choose to solve the challenge ahead of time and walk through their solution during the interview. Candidates who prefer to live code are strongly encouraged to review the challenge ahead of time, and are free to use any prepared notes during the interview. Candidates who prefer to fully develop a solution ahead of time should be ready to discuss and potentially make changes to their solution with their interviewer.

## Getting Started

Begin the challenge by opening the `main.py` file in the Files view on the left. If the Files view is not already visible, click the Open Sidebar icon located at the top left of the screen, and look for the Files section in the pane that opens. Click the Files label to toggle between showing and hiding the project files.

Do not modify any file other than `main.py`.

## Requirements
- You will write a function with the input and outputs specified below.
- Your function must use at least one loop or iterator.
- Your function must use at least one conditional statement.
- Your function must use at least one Dictionary or List to store data. You should be familiar with the features of _**both**_ data types, even if you only use one in your function.
- The Python module math is imported and available to use but not required. Please do not import any additional modules (such as NumPy).

## Problem Statement
Ada's Flooring Superstore aims to run the best full-service flooring shop in the neighborhood. Ada boasts a range of elegant flooring materials and additional services and promotional discounts... Ada will NOT be undersold! With your help, Ada’s Flooring Superstore will have the speediest quote calculator in the industry.

- A quote is for only one room and one type of carpet. The options are berber, texture, or pattern. The respective prices per square foot are listed below.
- A quote has or more options. The options are 10 year warranty, delivery, installation, and stain guard. Their respective prices, which are a flat rate, i.e. not dependent on square footage, are listed below.
- Ada's Flooring is running a special on free installation for customers with the discount code "ADAROCKS". So, if a customer has a coupon code, don't include the installation cost in the quote total.
- The function called `carpet_quote_estimator` accepts four parameters:
  - `room`, a list of numbers representing the room's length and width in feet
  - `carpet_type`, a string representing the type of carpeting
  - `options`, a list of strings, representing 0 or more options 
  - `promo_code`, a string representing the discount code
- The function must print the price of the order in dollars (i.e., with two decimal places). Refer to the example output for the specific formatting.

### Carpet Type
|Name|Price ($) per square foot|
|----|---------|
| berber | 5.09 |
| texture | 3.69 |
| pattern | 2.89 |


### Options
|Name|Price ($)|
|----|---------|
| 10yr warranty | 100.00 |
| delivery | 35.00 |
| installation | 75.00 |
| stain guard | 30.00 |

## Examples

These examples are also provided as a set of tests that can be run from the Tests panel at the left (the icon appears under Tools, and looks like a check mark). Clicking the Run tests button will run the Challenge inputs against your code, displaying either a success message, or a message about what was expected and what was observed. You may need to open an additional Console view, and rerun the tests, in order to see the test result messages.

### Example 1
#### Input (arguments of the function)
```
room = [10, 10]
carpet_type = "berber"
options = ["delivery", "installation"]
promo_code = ""
```
#### Output (printed by the function)
```
The cost is $619.00
```

### Example 2
#### Input (arguments of the function)
```
room = [8, 10]
carpet_type = "texture"
options = ["delivery", "10yr warranty", "stain guard"]
promo_code = ""
```
#### Output (printed by the function)
```
The cost is $460.20
```

### Example 3
#### Input (arguments of the function)
```
room = [11, 9]
carpet_type = "pattern"
options = ["delivery", "installation", "10yr warranty", "stain guard"]
promo_code = "ADAROCKS"
```
#### Output (printed by the function)
```
The cost is $451.11
```

### Example 4
#### Input (arguments of the function)
```
room = [12, 14]
carpet_type = "texture"
options = []
promo_code = ""
```
#### Output (printed by the function)
```
The cost is $619.92
```
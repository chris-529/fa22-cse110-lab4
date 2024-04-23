# 1. What will happen at line 12 and why? If the code causes an error, explain why. 

Line 12 prints `3` because that is the value of `i` after the for loop ends (prices is a list with 3 elements). We have access to `i` still because we declared it with keyword `var`, so we can print it's value outside of the for-loop block scope.

# 2. What will happen at line 13 and why? If the code causes an error, explain why. 

Line 13 prints `150`, because that is the last value it was assigned to inside of the for-loop. We did 0.5 * the last item in prices and assigned that value to `discountedPrice`. Again, we have access to `discountedPrice` because we defined it with `var`.

# 3. What will happen at line 14 and why? If the code causes an error, explain why.

Line 14 prints `150` again, because we simply rounded down `discountedPrice` in the final loop iteration and it did not need any rounding, so it stayed at `150`. We have access to the `finalPrice` variable since it's inside of our block scope and defined with `var`.

# 4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.

This function will return the list `[50, 100, 150]`. This is because we passed in the list of `[100, 200, 300]`, a discount of `0.5` to the function as parameters, and multiplied each item in the original price list by the given discount. Then we add these new prices to a list to return.

# 5. What will happen at line 12 and why?  If the code causes an error, explain why. 

At line 12 an error occurs because we are trying to access variable `i` which has been declared with keyword `let`, so it is only accessible within the block scope it is in. That block scope is the for-loop body, and we are trying to print the value of it outside of the for-loop, so an error occurs.

# 6. What will happen at line 13 and why? If the code causes an error, explain why.

At line 13 an error occurs because we are trying to access variable `discountedPrice` which has been declared with keyword `let`, so it is only accessible within the block scope it is in. That block scope is the for-loop body, and we are trying to print the value of it outside of the for-loop, so an error occurs.

# 7. What will happen at line 14 and why? If the code causes an error, explain why.

At line 14, the code prints `150`. This is because, although `finalPrice` is declared with `let`, it is declared inside of the scope we are accessing it's value. The scope of `finalPrice` is the entire function body. So it is fine. Inside of the for-loop we simply update it's value by doing 300 * discount.

# 8. What will this function return? Give a brief explanation. If the code causes an error, explain why.

The function returns a list, `[50, 100, 150]`. This is because, like the previous explanation, we call the function with two parameters: prices (`[100, 200, 300]`), and discount (.5). So we apply the discount to each item in the list in the for loop, add the new discounted price to a list, and return the new price list at the end of the function on `line 16`.

# 9. What will happen at line 11 and why? If the code causes an error, explain why.

At line 11 we will get an `Uncaught ReferenceError` because we're trying to access variable `i`'s value outside of it's scope. `i` was declared with keyword `let`, so we cannot access it outside of the for-loop body.

# 10. What will happen at line 12 and why? If the code causes an error, explain why. 

At line 12, the console will print `3`, because we are accessing `const length` inside of it's scope, so we have a reference to it. It is defined with `const`, so just printing it's vallue is allowed and will not cause an error. It has a value of 3 because we called the function with a list of 3 elements and assign the length of that list to `const length`.

# 11. What will this function return? Give a brief explanation. If the code causes an error, explain why. 

This function will return the list `[50, 100, 150]`. This is because we passed in the list of `[100, 200, 300]`, a discount of `0.5` to the function as parameters, and multiplied each item in the original price list by the given discount. Then we add these new prices to a list to return.

# 12. Given the above Object, write the notation for:

Accessing the value of the name property in the student object: `student.name`

Accessing the value of the Grad Year property in the student object `student['Grad Year']`

Calling the function for the greeting property in the student object `student.greeting();`

Accessing the name property of the object in the Favorite Teacher property in student `student['Favorite Teacher'].name`

Access index zero in the array of the courseLoad property of the student object `student.courseLoad[0]`

# 13. Arithmetic

A. ‘3’ + 2

Output: `'32'`
Reason: Integers map to their string representation, so we are appending the string `2` to `3` to get `32`

B. ‘3’ - 2

Output: 1
Reason: We are performing subtraction, which is not really defined for strings, so the `'3'` string gets converted to an integer and then we perform `3 - 2 = 1`

C. 3 + null

Output: `3`
Reason: `null` maps to `0` , so adding 0 to the number 3 will give 3

D. ‘3’ + null

Output: `'3null'`
Reason: This time, we have a string `'3'` and add null to it. So null maps to a string, not a number, which means null maps to `'null'` and we perform stringwise addition

E. true + 3

Output: `4`
Reason: Since we are performing addition on a number and a boolean, the boolean maps to it's numeric value (true = 1), and we add the two numbers to get 4

F. false + null

Output: `0`
Reason: Both `false` and `null` map to the numeric value of `0`, so we perform `0 + 0 = 0`

G. '3' + undefined

Output: `'3undefined'`
Reason: We are performing addition to a string `'3'` with `undefined` which maps to the string `'undefined'`, and the stringwise addition gives us the output

H. '3' - undefined

Output: `NaN`
Reason: `undefined` cannot be mapped to a numeric value, so we get `NaN` which means not a number. 

# 14. Comparison

A.‘2’ > 1

Output: `true`
Reason: This is a comparison of two different types so they get converted to numeric values, and the numeric 2 is > 1, so true.

B. ‘2’ < ‘12’

Output: `false`
Reason: This is a string and string comparison so they remain as strings, and the first character `2` is not lexicographically smaller than `1`, so we know it to be `false` immediately

C. 2 == ‘2’

Output: `true`
Reason: `'2'` gets converted to a numeric 2, and so we are saying numeric 2 is equal to numeric 2 which is true.

D. 2 === ‘2’

Output: `false`
Reason: The `===` operator performs an equality check without a conversion, and these are different types so we get false.

E. true == 2

Output: `false`
Reason: `true` gets converted to its numeric equivalent numeric value 1, and numeric 1 does not equal numeric 2 so we get false.

F. true === Boolean(2)

Output: `true`
Reason: `Boolean(2)` gets converted to `true` because it is a "non-empty value", and boolean true does equal boolean true

# 15. Explain the difference between the == and === operators.

The difference between `==` and `===` is that `===` does an equality check without converting the type of the two operands at all. So if you're comparing two operands that are of different type, you will surely get false back. For example, `'2' === 2` returns false while `'2' == 2` returns true. 

# 16. See file


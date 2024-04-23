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




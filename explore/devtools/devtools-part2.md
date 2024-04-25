# 1. What was the bug?

The bug is that the numbers we type in are of type string when we access the .value of the text area, instead of type number.

# 2. How would you fix it?

I fixed the bug by adding parseInt() around the lines for num1 and num2 where we extract the value of the input field. This will convert the string to a number as we desire.

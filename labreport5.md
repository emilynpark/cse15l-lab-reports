Response from TA: You have the right idea that there is an error in the logic behind the division in the return statement.
`arr.length` gives us the length of the entire array. When the method calculates the average without the lowest
number, the occurrence of the lowest number shouldn't be included as part of the calculation. Therefore, you
need to revise the divisor of the return statement(hint: you should subtract a certain number from arr.length; hopefully this
number is obvious based off of the explanation in the previous sentences!).

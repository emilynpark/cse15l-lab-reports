# Lab Report 5

## Debugging Scenario


## Response from TA:
<br>You have the right idea that there is an error in the logic behind your implementation. You will need to implement a way to identify the first instance of the lowest element in order for your tests to run as expected. One way in which you can achieve this is by initializing a boolean variable with the name `found` and initially setting it to false, and then in your second for loop you can implement code to check whether or not the lowest number in the array has been located. If the current `num` that is being checked by the for loop isn't equal to the lowest number, or if the lowest number has already been found(if the value of `found` is equal to true at this point), then the lowest number gets added to the total sum. If the current `num` that is being checked by the for loop is equal to the lowest number, and if the lowest element hasn't yet been located(if the value of `found` is equal to false at this point), then `found` should be set to true.</br>
<br>Additionally, there is an error behind the logic in the division in your return statement. `arr.length` gives us the length of the entire array. The occurrence of the lowest number shouldn't be included as part of the calculation. Therefore, you need to revise the divisor of the return statement(hint: you should subtract a certain number from arr.length; refer to the explanation in the previous sentences to figure out the correct number to subtract).</br>

## Response from Student:


1. Line 12 will print: 3 Because i gets incremented after each iteration of for loop, and end with 3 because the prices variable has a length of 3, also i is declared with var, which provides the function scope, so i can be accessed outside the for loop.
2. Line 13 will print: 150 Because discountedPrice gets updated to be 300 * (1 - 0.5) = 150 in the last iteration of the for loop, also discountedPrice is declared with var, which provides the function scope, so discountedPrice can be accessed outside the for loop.
3. Line 14 will print: 150 Because finalPrice gets updated to be Math.round(discountedPrice * 100) / 100 in the last iteration of the for loop, which has the same value as discountedPrice. Math.round takes no effect since it is already an integer. Also finalPrice is declared with var, which provides the function scope, so finalPrice can be accessed by any code within this function.
4. This function returns a list [ 50, 100, 150 ] because in each iteration of the for loop, the finalPrice gets pushed to discounted variable, which means 50 gets pushed when i = 0, 100 gets pushed when i = 1, and 150 gets pushed when i = 2. The calculation for discountedPrice and finalPrice was explained in answers for question 2 and 3. Also discounted is declared with var, which provides the function scope, so discounted can be accessed by any code within this function.
5. Line 12 results in ReferenceError because variable i is defined with let, which can only be accessed within the for loop. There it cannot be accessed by line 12, and resulting in an error.
6. Line 13 results in ReferenceError because variable discountedPrice is defined with let, which can only be accessed within the for loop. There it cannot be accessed by line 13, and resulting in an error.
7. Line 14 will print: 150 Because finalPrice gets updated to be Math.round(discountedPrice * 100) / 100 in the last iteration of the for loop, which has the same value as discountedPrice. Math.round takes no effect since it is already an integer. Although finalPrice is declared with let, it can be accessed within the for loop because the for loop is in the same block as the finalPrice variable. Therefore, no error is caused by Line 14.
8. This function returns a list [ 50, 100, 150 ] because in each iteration of the for loop, the finalPrice gets pushed to discounted variable, which means 50 gets pushed when i = 0, 100 gets pushed when i = 1, and 150 gets pushed when i = 2. The calculation for discountedPrice and finalPrice was explained in answers for question 2 and 3. Although discounted is declared with let, it can be accessed within the for loop because the for loop is in the same block as the discounted variable. Therefore, no error is caused by the code.
9. Line 11 results in ReferenceError because variable i is defined with let, which can only be accessed within the for loop. There it cannot be accessed by line 11, and resulting in an error.
10. Line 12 will print: 3 Because length does not get changed after declaration at all. Although length is declared with const, which provides the block scope, it can be accessed in the for loop because for loop is in the same block as length, therefore, no error is caused by this code.
11. This function returns a list [ 50, 100, 150 ] because in each iteration of the for loop, the discountedPrice gets pushed to discounted variable, which means 50 gets pushed when i = 0, 100 gets pushed when i = 1, and 150 gets pushed when i = 2. The calculation for discountedPrice was explained in answer for question 2. Although discounted is declared with const, it cannot be modified to another array, but the array itself can still be modified, meaning you can push elements to it. Therefore no error is caused by the code.
12. 
a. student.name
b. student[‘Grad Year’]
c. student.greeting()
d. student[‘Favorite teacher’].name
e. student.courseLoad[0]
13. Arithmetic
a. ‘3’ + 2			’32’ because 2 gets converted to string

b. ‘3’ - 2			1 because 3 gets converted to number

c. 3 + null			3 because null gets converted to 0

d. ‘3’ + null		‘3null’ because null gets converted to string

e. true + 3		4 because true gets converted to 1

f. false + null		0 because both false and null get converted to 0

g. ‘3’ + undefined	‘3undefined’ because undefined gets converted to string

h. ’3’ - undefined	NaN because undefined gets converted to not a number
14. Comparison
a. ‘2’ > 1				true because ‘2’ is converted to number 2

b. ‘2’ < '12'			false because ‘2’ is greater than ‘1’ in lexicographical order

c. 2 == '2'			true because ‘2’ is converted to number 2

d. 2 === '2'			false because of strict comparison that checks the equality without type conversion

e. true == 2			false because true is converted number 1

f. true === Boolean(2)	true because Boolean(2) is evaluates to true

15. == is a regular equality operator that converts different types to a common type when comparison, while === is a strict equality operator that checks the equality without type conversion.

17. The result of modifyArray([1,2,3], doSomething), will be a list of [2, 4, 6] because [1, 2, 3] is passed to be array, and doSomething is passed to be callback, in each iteration of the for loop, it would perform newArr.push(doSomething(array[i])), for example when i = 2, it would be newArr.push(doSomething(array[2])), since array[2] is 3, and doSomething(3) is 6, it is actually pushing 6 to newArr.

19. The output is 1 4 3 2.

## Question 1:

The following is printed by line 12:

> 3

## Question 2:

The following is printed by line 13:

> 150

## Question 3:

The following is printed by line 14:

> 150

## Question 4:
The function does not print anything. However, we know that the function returns
an array of integers **discounted**. In this case, we know that **discounted =
[50, 100, 150]**.

## Question 5:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question5.js:12
>     console.log(i);
>                 ^
> 
> ReferenceError: i is not defined
>     at discountPrices (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question5.js:12:17)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question5.js:19:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

This is because the **let** keyword has a block scope. This means that the
variable **i** is only accessible within the for loop that begins on line 6
and ends on line 10. Therefore, a ReferenceError is thrown.

## Question 6:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question6.js:13
>     console.log(discountedPrice);
>                 ^
> 
> ReferenceError: discountedPrice is not defined
>     at discountPrices (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question6.js:13:17)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question6.js:19:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

This is because the **let** keyword has a block scope. This means that the
variable **discountedPrice** is only accessible within the each loop of the 
for loop that begins on line 6 and ends on line 10. Therefore, a 
ReferenceError is thrown.

## Question 7:

The following is printed by line 14:

> 150

## Question 8:
The function does not print anything. However, we know that the function returns
an array of integers **discounted**. In this case, we know that **discounted =
[50, 100, 150]**.

## Question 9:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question9.js:11
>     console.log(i);
>                 ^
> 
> ReferenceError: i is not defined
>     at discountPrices (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question9.js:11:17)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part2/part2-question9.js:17:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

This is because the **let** keyword has a block scope. This means that the
variable **i** is only accessible within the for loop that begins on line 6
and ends on line 9. Therefore, a ReferenceError is thrown.

## Question 10

The following is printed by line 12:

> 3

## Question 11
The function does not print anything. However, we know that the function returns
an array of integers **discounted**. In this case, we know that **discounted =
[50, 100, 150]**.

## Question 12a)
Accessing the value of the **name** property in the student object can be
accomplished as such:

> let studentName = student.name;
> console.log(studentName); // logs 'Sarah'

## Question 12b)
Accessing the value of the **'Grad Year'** property in the student object can be
accomplished as such:

> let gradYear = student.['Grad Year'];
> console.log(gradYear); // logs '2022'

## Question 12c)
Calling the function for the **greeting** property in the student object can be
accomplished as such:

> student.greeting(); // logs 'Hello!'

## Question 12d)
Accessing the **name** property of the object in the **'Favorite Teacher'** 
property in the student object can be accomplished as such:

> let favoriteTeacherName = student.['Favorite Teacher'];
> console.log(favoriteTeacherName); // logs 'Thomas Powell'

## Question 12e)
Accessing the zero index in the array of the **courseLoad** property of 
the student object can be accomplished as such:

> let firstCourse = student.courseLoad[0];
> console.log(firstCourse); // logs 'CSE 110'

## Question 13a)
The following output is given:

> 32

The '+' operator is used to concatenate the string '3' with the number '2',
resulting in the string '32'.

## Question 13b)
The following output is given:

> 1

The '-' operator is used to subtract the number '2' from the string '3'.
JavaScript converts the string to a number and performs integer subtraction,
resulting in the number '1'.

## Question 13c)
The following output is given:

> 3

When the '+' operator is used with a number and 'null', the 'null' is turned
into the number '0'. Therefore '3 + null' results in the number '3'.

## Question 13d)
The following output is given:

> 3null

The '+' operator is used to subtract the number '2' from the string '3'.
JavaScript converts the string to a number and performs integer subtraction,
resulting in the number '1'.

## Question 13e)
The following output is given:

> 4

When the '+' operator is used with a boolean and a number, 'true' is turned
into the number '1'. Therefore 'true + 3' returns the number '4'.

## Question 13f)
The following output is given:

> 0

When the '+' operator is used with a boolean and 'null', 'false' is turned
into the number '0'. From 13c we konw that when 'null' is used with a number,
the 'null' is turned into a number '0'. Therefore 'false + null' returns a
number '0'.

## Question 13g)
The following output is given:

> 3undefined

The '-' operator is used to subtract the number '2' from the string '3'.
JavaScript converts the string to a number and performs integer subtraction,
resulting in the number '1'.

## Question 13h)
The following output is given:

> NaN

The '-' operator is used to subtract 'undefined' from the string '3'.
However, JavaScript cannot perform subtraction with 'undefined', so the result
is 'NaN' or not a number.

## Question 14a)
The following output is given:

> true

When comparing a string and a number, JavaScript automatically converts the
string into a number before performing the comparison. Here the string '2' 
is converted to the number 2 which is greater than 1, returning true.

## Question 14b)
The following output is given:

> false

When comparing two strings, JavaScript performs a character-by-character
comparison of the ASCII characters in the two strings. In this case, the first
character of '2', '2' has an ASCII value of 50 which is greater than that of 
the first character of '12', which has an ASCII value of 49. Therefore, the
comparison returns false.


## Question 14c)
The following output is given:

> true

The '==' operator in JavaScript comparison performs type coercion. Therefore the
string '2' is converted into the number 2. Thus, the expression is equivalent to
'2 == 2', which will output true.

## Question 14d)
The following output is given:

> false

The '===' operator in JavaScript compares both the value and the type of its
operands. Since the operands have different types (string and number), the
expression will evaluate to false.

## Question 14e)
The following output is given:

> false

Here, the boolean 'true' is converted into the number 1. Therefore, '1 == 2'
will return false.

## Question 14f)
The following output is given:

> true

Here, the boolean function is applied to the number '2'. Since the boolean
function returns 'true' for any nonzero number, 'true == true' returns true.

## Question 15
The '===' operator compares both the value and the type of its operands. On the
other hand, the '==' operator performs type coercion. This is seen in the
question 14.

## Question 16
Solution can be found in the '/part2/part2-question16.js'.

## Question 17
The following output is given:

> [2, 4, 6]

Two functions, modifyArray and doSomething are defined. We see that doSomething
simply return two times the parameter. We see that modifyArray calls the
callback function on every element in an array that is passed in. Therefore,
calling modifyArray([1,2,3], doSomething) multiplies every element in the array
by two.

## Question 18
Solution can be found in the '/part2/part2-question18.js'.

## Question 19
The following output is given:

> 1
> 4
> 3
> 2

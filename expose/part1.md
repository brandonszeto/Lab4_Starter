## Question 1:

The following is printed by line 9:

> values added: 20

## Question 2:

The following is printed by line 13:

> final result: 20

## Question 3:

The following is printed by line 9:

> values added: 20

## Question 4:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question3.js:13
>     console.log('final result: ', result);
>                                   ^
> 
> ReferenceError: result is not defined
>     at sumValues (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question3.js:13:35)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question3.js:16:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

This is because the **let** keyword has a block scope. This means that the
variable result is only accessible within the if statement that begins on line 3
and ends on line 11. Therefore, a ReferenceError is thrown.

## Question 5:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:7
>         result = num1 + num2;
>                ^
> 
> TypeError: Assignment to constant variable.
>     at sumValues (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:7:16)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:16:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

This is because the **const** keyword prevents the variable **result** from being reassigned after it
is assigned for the first time. Therefore on line 7, when the code attempts to
reassign result to num1 + num2, a TypeError is thrown.

## Question 6:

The following error is thrown:

> /Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:7
>         result = num1 + num2;
>                ^
> 
> TypeError: Assignment to constant variable.
>     at sumValues (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:7:16)
>     at Object.<anonymous> (/Users/brandonszeto/Documents/Class/CSE-110/Lab4_Starter/expose/part1-question5.js:16:1)
>     at Module._compile (node:internal/modules/cjs/loader:1267:14)
>     at Module._extensions..js (node:internal/modules/cjs/loader:1321:10)
>     at Module.load (node:internal/modules/cjs/loader:1125:32)
>     at Module._load (node:internal/modules/cjs/loader:965:12)
>     at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:83:12)
>     at node:internal/main/run_main_module:23:47
> 
> Node.js v20.0.0

Similarly to question 6, the **const** keyword prevents the variable **result** 
from being reassigned after it is assigned for the first time. Therefore on line 
7, when the code attempts to reassign result to num1 + num2, a TypeError is 
thrown. However, additionally, the **const** keyword has the same scope as the 
**let** keyword. This means that the scope of the variable **result** is within 
the if statement that begins on line 7 and ends on line 11. Thus, from even if 
there was no TypeError, a ReferenceError would be thrown.

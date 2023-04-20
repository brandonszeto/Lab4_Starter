# DevTools Part 2

1. The bug was that num1 and num2 were being concatentated rather than being
   added as intended.
2. I would fix it by changing line 11 to the following line:
> let result = parseInt(num1) + parseInt(num2);

1. The bug is that the values of ```num1``` and ```num2``` are both strings, which in turn sets ```result``` to be a string by concatenation.
2. I would fix this by ensuring that num1 and num2 are both number values rather than strings, which can be done by using the ```parseInt()``` function with base 10. 

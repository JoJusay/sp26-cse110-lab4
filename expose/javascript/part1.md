1. Line 9 prints ```values added: ``` followed by the result of adding num1 and num2.
2. Line 13 would print ```final result: ``` followed by 0, since result was declared with var inside of the if statement with 0.
3. We should not use ```var``` because it ignores the block scope and can result in naming conflicts or with incorrect values from outside of the blocking. In some instances it can lead to incorrect initialization and undefined behavior.
4. Line 9 would print ```values added: ``` followed by the result of adding num1 and num2.
5. Line 13 would return an error since ```let``` is block-scoped, so in the else portion, ```result``` is undefined.
6. Line 9 would print ```values added: ``` followed by the 0, since ```result``` cannot be changed after being declared using ```const```.
7. Line 13 would return an error since ```const``` is block-scoped just like ```let```, so in the else portion, ```result``` is undefined.

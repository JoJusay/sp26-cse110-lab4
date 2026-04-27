1. Line 12 would log ```prices.length``` since ```i``` was declared as ```var```, meaning it is not restricted to the for loop.
2. Because ```discountedPrice``` was declared as ```var```, and line 13 takes place after the for loop, line 13 would log the last declaration of ```discountedPrice```.
3. ```finalPrice``` was declared with ```var```, and it was used inside of the for loop, so line 14 would log the last declaration of ```finalPrice``` from the for loop.
4. The function will return an array of values that were calulated in the for loop. Because it was defined as ```var``` and because values were pushed into it, there would not be any errors in returning it.
5. Line 12 would return an error. Because ```i``` was declared in the for loop using ```let```, its existence is contained only when the for loop is running and therefore it no longer exists outside of it.
6. Line 13 would also return an error. Because it was defined using ```let```, it only exists within the block it was decalred in, that being the for loop. Because line 13 is after the for loop, ```discountedPrice``` no longer exists, so attempting to log it would cause an error
7. This would not result in an error and would instead properly log what ```finalPrice``` was at the end of the for loop. It was declared using ```let``` within the function block, so logging it would not cause errors since line 13 is in the same scope.
8. The function will return an array of values that were calulated in the for loop. Because it was defined as ```let``` in the same scope as the return statement, and because values were pushed into it in the for loop, there would not be any errors in returning it.
9. Line 11 would return an error. Because ```i``` was declared in the for loop using ```let```, its existence is contained only when the for loop is running and therefore it no longer exists outside of it, hence using ```i``` as undefined would cause an error.
10. Line 12 would log ```length``` properly. The length is not changed at all so the use of ```const``` is valid. Because it was also declared in the same scope as line 12, there would be no problems with accessing it and logging it.
11. The function will return an array that has been properly populate. ```discounted``` is a ```const``` variable, meaning that the entire array cannot be reassigned, but the contents itself can be changed, so ```discounted``` is properly allocated.
12. A:```student.name```, B: ```student["Grad Year"]```, C:```student.greeting()```, D:```student["Favorite Teacher"].name```, E:```student.courseLoad[0]```
13. Arithmetic:
    - A: ```'3' + 2 = '32```. This is because the ```2``` maps directly to a string and the ```+``` concatenates the two strings.
    - B: ```'3' - 2 = 1```. This is because the ```'3'``` maps to the integer ```3```, so substraction is performed.
    - C: ```3 + null = 3```. ```null``` is equivalent to the integer ```0```, so we are performing addition.
    - D: ```'3' + null = 3null```. This is because ```null``` is converted into a string, so the ```+``` works as concatenation.
    - E: ```true + 3 = 4```. This is because ```true``` maps to the value ```1```, so the ```+``` works as addition.
    - F: ```false + null = 0```. Neither of the two are declared as strings, so they are converted into integers. Both ```false``` and ```null``` map to ```0```, so we get ```0``` when adding.
    - G: ```'3' + undefined = 3undefined```. The ```undefined``` gets converted into a string and gets concatenated with the 3.
    - H: ```'3' - undefined = NaN```. There is no string operator with ```-```, so the 3 gets converted into an integer. Because ```undefined == NaN```, we get ```NaN``` by subtracting it from 3.
14. Comparison:
    - ```'2' > 1 --> true```. ```2``` is converted to an integer, and ```2 > 1```, so ```true``` is returned.
    - ```'2' < '12' --> false```. This compares the characters of each string to check the lexographical order. Because the first character ```'2'``` does ont come after ```'1'```, we get ```false```.
    - ```2 == '2' --> true```. This converts the two arguments to the same type. Because they are equivalent in casting to both integers and strings, we get ```true```.
    - ```2 === '2' --> false```. This compares their datatypes. Because the datatypes are not the same, ```false``` is returned.
    - ```true == 2 --> false```. ```true``` maps to ```1```, and because ```1``` and ```2``` are not the same, false gets returned.
    - ```true === Boolean(2) --> true```. ```Boolean(2)``` converts to true if the value is not empty, ```null```, ```0```, ```NaN```, or ```undefined```, the comparison between the two arguments returns ```true```.
15. ```==``` compares two values and allows for type conversions to check if they are equivalent. ```===``` does not allow for type conversions and only compares two values as they are given, so if they do not match data types then the value will be ```false```
16. **ANSWERED IN ```part2-question16.js```**
17. The result of this ```modifyArray([1,2,3], doSomething)``` is an array ```[2,4,6]```. On the initial call, a new array aptly named ```newArr``` is allocated as empty. Then we iterate through the ```array``` parameter and perform the ```callback``` parameter function on it, followed by pushing the result onto ```newArr```. Because ```doSomething``` was passed as the ```callback``` parameter, we are performing doubling onto each othe the values in ```array```, so the values of ```newArr``` are double that of the values in ```array```.

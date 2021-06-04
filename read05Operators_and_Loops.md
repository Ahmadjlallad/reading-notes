#### Operators and Loops:
- Operators:performs some operation on single or multiple operands (data value) and produces a result.
  * Compound assignment operators my favorite type there are a lot of that for example ```x &&= y``` it means  ```x && (x = y)``` this type allows  you to shortens the code, you can check it on the internet
  * Return value and chaining
    - The return value matches the expression to the right of the ```=``` sign in the “Meaning” column of the table above this for mathematical.
    - logical assignments return value is that of the logical operation without the assignment, return values based on the operands’ values before the operation.
  * Destructuring makes it possible to extract data from arrays or objects using a syntax ```var foo = ['one', 'two', 'three'] // without destructuringvar one   = foo[0];var two   = foo[1];var three = foo[2];// with destructuringvar [one, two, three] = foo;``` helpfull untheless
  * Bitwise operators(logical) (```&``` and, ```|``` or, ```^```Xor ```~```not )
   - for ever one of this logical opreters there is some thaing called truth table And for example

|X|Y|And result| or result|xor result|
|-|-|-|-|-|
0|0|0|0|0
0|1|0|1|1
1|0|0|1|1
1|1|1|1|0
  
  - the idea is the two inputs must be true ```OR |``` on the hand one of the input must be true to get true ```Xor ^``` outouts true if the two input values differ.
* Loops and iteration
  * For repeats until a specified condition evaluates to ```false```. The JavaScript for loop is similar to the Java and C for loop.```for ([initialExpression]; [conditionExpression]; [incrementExpression])statement```
   *If the value of ```conditionExpression``` is true, the loop statements execute. If the value of ```condition``` is false, the for loop terminates. 
  * while loop ```while (condition) statement```false, statement within the loop stops executing.
### In general, you should use a for loop when you know how many times the loop should run. If you want the loop to break based on a condition other than the number of times it runs, you should use a while loop.
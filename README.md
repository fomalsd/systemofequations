# System of Equations 
Test task for Clarity AI

The system of equations will consist of an unspecified number of equations formatted like:
```
varname = [ number1 | varname1 ] { ^ [ number2 | varname2 ] } { ^ [ number3 | varname3 ] } ... 
```
Where:
**varname** is made up of letters. Example: a, ke, ikall 
**number** is a integer number
^ represents the operator XOR (Exclusive OR). XOR operator is a bitwise operator that compares the bits one by one and returns 0 if the matching bits are the same and returns 1 if the matching bits are different (not the same) 

Each equation represents an assignment (=) that sets a value to the var varname. The list of equations will be passed as a String whose equations are separated by a semi-colon and a blank (‘; ‘). In addition, the following assumptions can be made: 

The same var cannot be on the left side of multiple equations, just on one or none. The equations do not follow any particular order. Your function must find the value of the variable “x”. When the solution is impossible to be reached, the function will return the string null. 

Your function must find the value of the variable “x”. When the solution is impossible to be reached, the function will return null.

## Examples
```
Input: "c = 3717 ^ 8396 ^ 4987; x = x; u = d ^ c; d = 4144; e = q"
Output: 4144
```
```
Input: "y = 6 ^ z; z = y ^ 2; x = z ^ y ^ 3"
Output: null
```

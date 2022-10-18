# "Training JS #6: Basic data types--Boolean and conditional statements if..else" #


### Task

>
Coding in function ```trueOrFalse```, function accept 1  parameters:```val```, try to use the conditional statement if...else, if ```val``` value is false (val==false or it can convert to false), should return a string "false", if not, return a string "true".
These values are converted to ```false``` in the conditional statement:
```
0, -0, "", null, undefined, NaN
```
>
### Solution

```
function trueOrFalse(val) {
  if (val == 0 || val == -0 || val == '' || val == null || val == undefined || val == NaN) return 'false';             
  else return 'true';
}
```

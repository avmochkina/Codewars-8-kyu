# "Training JS #14: Methods of Number object--toString() and toLocaleString()" #


### Task

>
Coding in function ```colorOf```. function accept 3 parameter:```r``` ```g``` ```b```. It means value of color red green and blue. the value range is 0-255.

Use ```toString(16)``` Convert numbers r g b to hex string form. at last, combine them to a web color code and return it.

the color code should starting with "#". and then use 2 characters per color.

for example:

```
colorOf(255,0,0) should return "#ff0000"
colorOf(0,111,0) should return "#006f00"
colorOf(1, 2 ,3) should return "#010203"

```
>

### Solution

```
function colorOf(r,g,b){
  let r16 = r.toString(16);
  let g16 = g.toString(16);
  let b16 = b.toString(16);
  
  if(r16.length < 2) r16 = "0" + r16;
  if(g16.length < 2) g16 = "0" + g16;
  if(b16.length < 2) b16 = "0" + b16;
  
  return "#" + r16 + g16 + b16;
}
```

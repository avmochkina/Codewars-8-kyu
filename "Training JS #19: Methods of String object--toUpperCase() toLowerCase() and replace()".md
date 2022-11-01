# "Training JS #19: Methods of String object--toUpperCase() toLowerCase() and replace()" #


### Task

>
Coding in function ```alienLanguage```, function accept 1 parameter:```str```. ```str``` is a sentence.

We translate the sentence into an alien language according to the following rules:

Each word in the sentence is separated by spaces. The last letter of each word in the sentence turns to lowercase, and the other letters are capitalized. Looks very strange? Because this is the form of alien language ;-)

for example:

```
alienLanguage("My name is John") should return "My NAMe Is JOHn"
alienLanguage("this is an example") should return "THIs Is An EXAMPLe"
alienLanguage("Hello World") should return "HELLo WORLd"
```
A small hint: The first conversion of the entire string will make the code easier
>

### Solution

```
function alienLanguage(str){
  let words = str.toUpperCase().split(" ");
  let result = [];
  for (let i = 0; i < words.length; i++) {
    let lastLetter = words[i][words[i].length-1].toLowerCase();
    result.push(words[i].slice(0, -1) + lastLetter);
  }
  return result.join(' ');
}
```

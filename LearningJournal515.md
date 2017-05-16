# Learning Journal
## May 15 2017
---
### The DOM
Today we've started learning the DOM (Document Object Model). What is the DOM? So apparently it is all the stuff on your page, which is arranged in a tree structure (ex: a <p> might live in <body> which lives in <html>)
>>The HTML DOM is a standard object model and programming interface for HTML. It defines:
>>The HTML elements as objects
>>The properties of all HTML elements
>>The methods to access all HTML elements
>>The events for all HTML elements
>>Definition credit: https://www.w3schools.com/js/js_htmldom.asp

_Aka, all the stuff that lives on your page_

### Loops
We also reviewed loops:
```
for (var i=0; i < 100; i++) {
//do something! like:
console.log('Cats are cool');
}
```
This says: for var i starting at the 0 and ending at 99, iterating by 1, log 'Cats are cool' to the console.

Here's another one:
```
for (var i = 2; i < 10; i--) {
console.log('Yo yo yo wazzup');
}
```
In this one we start iterating at 2 and end at 9, iterated DOWN by 1 each time the loop runs. When the loop runs, log "Yo yo yo wazzup" to the console.

Ok here is a while loop
```
while (i < 10) {
console.log('It's less than $10! You have to buy it!")
}
```
This one says while i (which I guess we defined outside of this loop somewhere) is less than 10, log to the console the stuff in (). Basically the loop stops when i = 10.
Here is a do while loop
```
do {
console.log('Yuck!')}
while (kale > 0)
```
So when var kale (which I assume we defined somewhere else) is greater than 0, the loop will log 'Yuck!'

### Object Literals
Objects in Javascript are basically just things, that have descriptions with them. I like to think of them as something you'd have to explain to a blind space alien.
Me: "Hey alien, this is a tree"
Queen Arignflirngoairnar of Planet Qiabgaiobfroa: "What's a tree? I'm not familiar?"
Me: "Well, it's got 10 branches, and 99 leaves, and it's bark is rough"

var tree = {
branches: 10,
leaves: 99,
bark: 'rough'
}

Another one for fun:
var jayZ = {
wife: 'Beyonce',
problems: 99,
girlproblems: 0,
notaproblem: 'b*tch',
hasGrammy: yes
}

Things I need to review tomorrow:
What the heck is going on with the nested functions in Friday's assignment? I keep looking at the code being like:
![BUT WHY](https://media.giphy.com/media/bsEujSWBjnNAI/giphy.gif)

Nonetheless:
![I WILL SOLVE YOU](https://media.giphy.com/media/3oz8xRdUokNRJ4qvF6/giphy.gif)

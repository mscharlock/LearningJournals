# Learning Journal
## May 10

![Seriously Loops, imma punch you in the face](http://dashie.mylittlefacewhen.com/media/f/img/mlfw1481_raritygrind.gif "LOOPS WHAT IS THE DEAL")

So I am still not sure what I am doing wrong with this loop thing today. I got one of them to work and then spent a bunch of time trying to get the other one to work. I figure that tomorrow all will be clear when Brian explains it but in the meantime, I am definitely feeling a little on the *deskflip!!* side.

With a little help, I got the first loop-ception to work for the "guess a number" type game. I think I am about 75% of the way to getting the other one to work, but still not sure why it isn't working.

Here's the number one:
```sh
//Guess a number
var myNumber;
var counter = 0;

while (myNumber !== 12) {
  myNumber = parseInt(prompt('What is my favorite number? Take a guess!'));

  if (myNumber > 50){
    alert('Too high!');
    counter++;
  } else if (myNumber < 3) {
    alert('Too low!');
    counter++;
  } else if (myNumber < 8 && myNumber > 20) {
    alert ('You\'re getting closer...');
    counter++;
  } else if (myNumber === 12) {
    alert('Yay, you win!');
  }

  if (counter === 4) {
    alert('Sorry, you ran out of tries - my favorite number is 12!');
    break;
  }
}

console.log('counter: ', counter);
```
So this one basically declares var myNumber (but doesn't define it), and declares/defines var counter as 0. Then it does a while loop. So WHILE myNumber isn't 12, then it'll prompt the user to enter a number (and force it to be a number by using parseInt) and if that number is greater than 50, it will say "Too high!" and log one to the counter. If the number is less than three, it will say "Too low!" and the counter will log one. If it's between 8 and 20, it'll say "You're getting closer" and log one on the counter. Finally if you actually guess the number, 12, then you get an alert that says "Yay! You win!" WHILE all that is going on, the counter is also controlled by an if statement. IF the counter equals 4, then it'll say you ran out of tries and break us out of the loop. Finally, we also log to the console that the var counter is counter just in case we forget/it becomes useful for debugging later.

Ok, here's the one with the while loop:
````sh
//Six tries to guess one of multiple answers
var ficCharas = ['Sherlock Holmes', 'Catwoman', 'Fluttershy', 'Xena'];
var flag;
var michelleFictionalCharacterBff = prompt('What fictional character would Michelle hang out with?');
console.log('michelleFictionalCharacterBff: ', michelleFictionalCharacterBff);

var guessCounter = 0;
console.log('guessCounter: ', guessCounter);

while (guessCounter <= 6) {
  for (var i=0; i < ficCharas.length; i++) {
    console.log('current guess: ', michelleFictionalCharacterBff);

    if (michelleFictionalCharacterBff === ficCharas[i]) {
      alert('Yay! You guessed right! All of the possible answers were: ' + ficCharas[i]);
      flag = true;
      break;
    }
    else if (!flag) {
      alert('No guess again!');
      guessCounter++;

    }
  }
}
````
So what this is doing is:
var ficCharas is an array of fictional characters I would hang out with.
var flag is set up but not defined.
var michelleFictionalCharacterBff is a prompt that asks who I would hang out with.
Then I'm console logging michelleFictionalCharacterBff so I can debug later.

Then I set up a guessCounter, equal to 0. And console logged it for posterity.

Then WHILE the guessCounter is less than or = to 6,
then I tried to set up a counter thing, which it turns out might be better outside of the while loop (see my 11 other attempts at this problem on Repl (https://repl.it/HsFT/11)). Then I tried an if - so it's if the answer matches something in the array, then alert, then flag it as true and break out of the loop. Otherwise, guess again and add to the counter.

I think I'm close but it's driving me bananas!!
I largely ignored CSS today because I was so focused on the loop thing. I do want to make the website look prettier though, since my ols and uls have now made it look kind of funky.

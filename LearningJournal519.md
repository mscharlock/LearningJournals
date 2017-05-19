## Learning Journal
### May 19 2017

Reviewing some basic concepts from this week:
## Object Literals
Declaring a thing right there and then with it's properties.
```
var cat {
    fuzzy: true,
    color: 'grey',
    stripey: 'yes'
    }
```

## Object Constructors
it's a FUNCTION that constructs objects
```
function Shoe {
    this.heel_height: heel_height;
    this.color: color;
    this.peeptoe: peeptoe;
    this.straps: straps; <-- I dunno
    }
```
to INSTANTIATE a NEW shoe, I use **new** with var for the thing
```
var sandal = new **S**hoe (1.5, 'yellow', 'no', ['4 on ankle', '2 around foot']
```

Let's do some more:
Let's make writers. The constructor function that's going to make them needs a capital letter **W**riter. Because we want to create stuff outside of this thing, we need to use the this to refer to it's interior stuff when we create a new one. So don't forget the thises.
```
function Writer {
    this.name = name;
    this.age = age;
    this.location = location;
    this.genre = genre;
    this.famousBook = famousBook;
    }

var shakespeare = new Writer ('Shakespeare', '30', 'England', 'plays', 'Romeo and Juliet');
var philipkdick = new Writer ('Philip K Dick', '45', 'USA', 'science fiction', 'A Scanner Darkly');
var emilydickenson = new Writer ('Emily Dickenson', '22', 'England? I acutally have no idea', 'poetery', 'Poem about something or other probably gardens');
```

## The DOM and getting stuff into it
The DOM is basically a representation of your HTML document. You can use JS to grab things from this representation and then put information into them.
```
var table = document.getElementbyId('awesomeTable') <-- Grab the thing
awesomeTable.addEventListener('click', function) --> I'd have to put a function in here so it actually does something when you click
```
document.getElementById() = a method that works on the document (the HTML) to grab something by it's ID which you put in the ()s
You have to grab the thing first, then you can do something with it
So you then take the thing the element and add an event listener, so it can lie in wait for a user to do whatever it is that you have specified it to do. Kinda like a birdwatcher? So the birdwatcher waits until a bird comes along and then logs it in their birding journal (this could be totally untrue, but let's pretend I know what I'm talking about for the sake of analogy). The birdwatcher is the event listener. The function is logging the bird in the journal.
But we have to make sure that the birdwatcher is like...in a place - for us, this is the DOM and the element.
```
So, the birdwatcher needs to watch in a field (so he can have a chance to actually see birds)
So we add event listener to a specific spot - the element we specified earlier by id.
document.getElementById('field')
field.addEventListener('bird shows up in binoculars', function log in your journal) <-- Something like this
```

Other concepts to review:
1. Forms
2. Tables
3. How events are working
4. What kinds of events there can be

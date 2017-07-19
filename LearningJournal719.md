# Learning Journal 
## July 19 2017 

Woo! Servers!

As a reminder to myself, here's what we talked about yesterday in terms of setting up servers: 
-in Terminal, run: 
```
npm init -y 
```
which sets up Node and gives you a basic json package that you can fill in later
OR 
```
npm init
```
which you then have to fill in. 
Then we have to set up body parser and express 
```
npm install -S express body-parser
```
should install both of them. 
Next we gotta set up the server.js file (so touch a new file) 
I also went ahead and moved all the static files into their own /public folder. 
In the server.js, we did: 
```
'use strict'
let express = require('express'); //we're requiring express and then assigning it into a variable//
let app = express();

const bodyParser = require('body-parser').urlencoded({extended: true}); , //still not totally sure what is happening here but basically we're requiring body-parser//
const PORT = process.env.PORT || 3000; //we're setting up a port in the environment or if that's not available, then use port 3000//

app.use(express.static('/public')); //make sure that express can get at your static files//

//we don't need this but we used it in our lab and essentially it is making a request related to the /notsurewhatgoeshere file - in lab it was the /articles file//
// app.post('/notsurewhatgoeshere', bodyParser, function(request, response) {
//   console.log(request.body);
//   response.send('Helloooo the server is listening to you!!');
// });

app.listen(PORT, function(){
  console.log(`'listening on port number: ${PORT}'`); //we are using the backtic notation to create a string/template literal and console log the port we are listening to. The literal stuff requires the ${} for particular stuff (objects??).//
});
```

I'm excited to delve into the rest of this stuff this week. I haven't done any backend really yet and I am excited to learn it. Also, there have been a lot more moment of "YES IT IS WORKING!" this week - I don't know why that feeling never kicked in in 201 but it is pretty exciting when you tell it to do something and then as if by magic, it really does it! 
Basically me when something works: 

![her face hahaha](https://media.giphy.com/media/l0MYw0DsFJc0kU0Jq/giphy.gif)

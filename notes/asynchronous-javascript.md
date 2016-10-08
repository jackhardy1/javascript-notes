### Asynchronous Javascript
_____

#### Index

<br>

[Asynchronous vs Synchronous](#asynchronous-vs-synchronous)

[The Event Loop](#the-event-loop)

<br>

#### Asynchronous vs Synchronous
_________

Synchronous: You want a pizza for dinner and you are out of the frozen kind. So you have to stop playing WOW which upsets your clan. You go to the kitchen, make the dough, cover it with sauce, add the cheese, and smother it your favorite bacon topping. You just spent 20 minutes of your time making the pizza with another 10 minutes in the oven. The timer beeps and you pull the hot pie out. You can sit back down in front of your computer, eat the pizza, and continue with your conquest.

Asynchronous: You want a pizza for dinner while playing WOW. You open up a browser window on your 5th monitor. You load up the Pizza website and order your extra cheesy bacon pizza with a side of bacon grease garlic sauce. You go back to your raid and after 20 minutes the door bell rings. You get the pizza. You sit back down in front of your computer, eat the pizza, and continue with your conquest.

”In programming, asynchronous events are those occurring independently of the main program flow. Asynchronous actions are actions executed in a non-blocking scheme, allowing the main program flow to continue processing.”

<br>

#### The Event Loop
______

Consider this example:

```console.clear();
console.log("a");
setTimeout(function(){console.log("b");},1000);
console.log("c");
setTimeout(function(){console.log("d");},0);
```
The outcome would be:

```
a c d b
```

Why?

### Tips ###

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  let response = "";

  if (hungry) {
    if (availableTime < 20) {
      response = "Let's pick up something to eat at our desk.";
    } else if (30 >= availableTime && availableTime >= 20) {
      response = "Let's try the sushi place nearby";
    } else {
      response = "Stop loafting. Let's get back to work.";
    }
  } else {
    response = "Since you're not hungry, get back to work.";
  }

  console.log(response);
};
```
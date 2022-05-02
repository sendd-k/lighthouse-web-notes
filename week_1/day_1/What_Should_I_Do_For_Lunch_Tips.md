### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === false) {
    console.log("Get back to work.")
  } else if (hungry === true && availableTime < 20) {
    console.log("Eat lunch in the lab.")
  } else if (hungry === true && availableTime < 30 && availableTime >= 20) {
    console.log("Try a place nearby.")
  } else if (hungry === true && availableTime > 30) {
    console.log("We are at bootcamp please reconsider your time managment.")
  }
}

function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```
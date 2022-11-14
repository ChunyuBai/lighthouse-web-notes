### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows:

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === true) {
    if (availableTime <= 20) {
      console.log(`pick up a snack or grab something you have ready at home.
      `);
    } else if (availableTime > 20 && availableTime <= 30) {
      console.log(`Take a break, should take time to cook.`);
    } else if (availableTime > 30) {
      console.log(`This is an intense program, should probably reconsider.`);
    }
  } else if (hungry === false) {
    console.log("No need to eat.");
  }
};
```
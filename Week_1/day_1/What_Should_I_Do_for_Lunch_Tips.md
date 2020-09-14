### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

``` javascript 
const whatToDoForLunch = function(hungry, availableTime) {
  let hungryBeginning = `I'm hungry and I only have ${availableTime} minutes for lunch.`;
  if (hungry === true) {
    if (availableTime < 20) {
      console.log(hungryBeginning + " I should pick something up and eat it in the lab!");
    }   else if (availableTime >= 20 && availableTime <= 30) {
      console.log(hungryBeginning + " Lets find somewhere nearby!");
    } else if (availableTime > 30) {
      console.log(hungryBeginning +  " But I shouldn't take such a long lunch!");
    }
  } else {
    console.log(`Although I have ${availableTime} minutes for lunch, I'm not hungry! Back to work!`);
  }
};
```
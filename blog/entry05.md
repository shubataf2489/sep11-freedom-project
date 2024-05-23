
# Process Writeup

## Name: Shubata Fizin
## Course: Javascript
## Period: 03
## Concept: p5js

### Context

In the spring term of my junior year, I learned the fundamentals of p5js. This learning period primarily revolved around essential concepts such as key, keyCode, keyPressed(), keyReleased(), keyTyped(), keyIsDown(), fill(), noFill(), noStroke(), stroke(), erase(), and noErase(). Each day, we delved into a new concept about p5js. We also used concepts we learned previously in DOM.

## Activities:

- **Classwork:** Assigned tasks during class helped me apply and reinforce the learned concepts.

- **Homework:** Homework assignments aided in consolidating the skills acquired during class.

- **Pong Remix:** Overcoming challenges in this activity clarified many misconceptions. The code brings out creativity in a classic ping pong game, focusing on concepts such as basics, movement, application, and pong.


```javascript
let x = 50; // Initial x-coordinate of the circle
let y = 50; // Initial y-coordinate of the circle
let speedX = 2; // Speed of movement in the x-direction
let speedY = 1; // Speed of movement in the y-direction

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);

  // Update the position of the circle
  x += speedX;
  y += speedY;

  // Draw the circle at its current position
  ellipse(x, y, 50, 50);

  // Reverse direction if the circle reaches the canvas edges
  if (x > width || x < 0) {
    speedX *= -1;
  }
  if (y > height || y < 0) {
    speedY *= -1;
  }
}
```
I had a hard time figuring out how to use this code.
```javascript
if (y > height || y < 0) {
    speedY *= -1;
  }
```
I initially struggled to understand how to incorporate the code for reversing direction when the circle reached the canvas edges. However, by referring to previous examples, I grasped the necessity of adding this functionality.

### [The p5js reference helped me a lot on this journey ](https://p5js.org/reference/)

```markdown
### keyCode
- `keyCode` is a variable in p5.js that stores the Unicode value of the most recent key pressed.

### Example:
```javascript
function draw() {
  if (keyCode === UP_ARROW) {
    // Do something when the up arrow key is pressed
  }
}
```

### keyPressed()
- `keyPressed()` is a function in p5.js that is called once whenever a key is pressed.

### Example:
```javascript
function keyPressed() {
  if (key === ' ') {
    // Do something when the spacebar is pressed
  }
}
```

### keyReleased()
- `keyReleased()` is a function in p5.js that is called once whenever a key is released.

### Example:
```javascript
function keyReleased() {
  if (key === 'a') {
    // Do something when the 'a' key is released
  }
}
```

### keyTyped()
- `keyTyped()` is a function in p5.js that is called once whenever a key that produces a character value is pressed.

### Example:
```javascript
function keyTyped() {
  if (key === 'h') {
    // Do something when the 'h' key is typed
  }
}
```

### keyIsDown()
- `keyIsDown()` is a function in p5.js that returns true if the specified key is currently pressed down.

### Example:
```javascript
function draw() {
  if (keyIsDown(LEFT_ARROW)) {
    // Do something while the left arrow key is held down
  }
}
```

### fill()
- `fill()` is a function in p5.js that sets the color used to fill shapes.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  fill(255, 0, 0); // Sets fill color to red
  rect(100, 100, 50, 50); // Draws a red rectangle
}
```

### noFill()
- `noFill()` is a function in p5.js that disables filling shapes with color.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  noFill(); // Disables fill color
  rect(100, 100, 50, 50); // Draws an unfilled rectangle
}
```

### stroke()
- `stroke()` is a function in p5.js that sets the color used to draw lines and borders of shapes.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  stroke(0); // Sets stroke color to black
  rect(100, 100, 50, 50); // Draws a rectangle with black border
}
```

### noStroke()
- `noStroke()` is a function in p5.js that disables drawing lines and borders of shapes.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  noStroke(); // Disables stroke
  rect(100, 100, 50, 50); // Draws a rectangle without border
}
```

### erase()
- `erase()` is a function in p5.js that sets the erasing mode, which allows shapes to be erased from the canvas.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  erase(); // Enables erasing mode
  rect(100, 100, 50, 50); // Erases a rectangle from the canvas
  noErase(); // Disables erasing mode
}
```

### noErase()
- `noErase()` is a function in p5.js that disables the erasing mode.

### Example:
```javascript
function setup() {
  createCanvas(400, 400);
  erase(); // Enables erasing mode
  rect(100, 100, 50, 50); // Erases a rectangle from the canvas
  noErase(); // Disables erasing mode
  rect(200, 100, 50, 50); // Draws a normal rectangle
}
```


### Takeaway:

My exploration of p5.js not only introduced me to fundamental concepts in creative coding but also helped with  my problem-solving skills. By experimenting with code and tackling challenges, I gained a deeper understanding of how to bring my creative ideas to life through programming. This experience not only expanded my technical knowledge but also inspired me to continue exploring the endless possibilities of coding in the realm of art and interactive design. I also learned how to use keyIsDown(), fill() properly.

### Next Steps:

Continuing to experiment with p5.js and exploring its vast potential for creating interactive visualizations and artistic projects. Further practice will deepen my understanding and enable me to undertake more complex coding challenges.


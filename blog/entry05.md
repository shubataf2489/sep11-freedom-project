
# Process Writeup

## Name: Shubata Fizin
## Course: Javascript
## Period: 03
## Concept: p5js

###  Context/Engineering Design Process

The engineering design process I'm currently engaged in involves communicating our results with my partner. We are both testing and refining our projects. Currently, we are discussing what went well and what we should have worked on in our project. The biggest thing I learned is the importance of being confident in your work. I also learned that confidence comes from fully understanding your work and a bit of acting. During the presentation, I improvised and changed what I was going to say a couple of times. I focused on improving my weak points, such as eye contact and speaking loudly enough. I was confident that I could explain well, so I didn't worry too much about that aspect. Another thing that helped ease my nerves was knowing my classmates and realizing that in a few minutes, this presentation would be over.

During the expo, I had to adjust my elevator pitch based on my audience. For instance, when presenting to judges, eleventh graders, and some sophomores, I adapted my approach. I would incorporate friendly jokes to maintain my peers' attention or shorten the part of my speech where I explained my challenges. I also realized the importance of communicating every step of the project when working with others and leaving extra time for any unforeseen challenges.


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

### Skill:

Time management: We both followed a strict schedule and both worked on our project at different times when we couldn't work together and when we could we would share  our discoveries.


Communication: I had to communicate and collaborate and share my findings with my partner on many occasions to ensure we were on the same page. As I have mentioned before, every weekend my partner and I call each other and share our screen every time we code to show each other what we are doing. Calling each other makes us accountable to do the work. Each week we alternate on who leads. On week one, Shelly took the lead on selecting a background that will be best for our game and I listed the pros and cons of each setting. Shelly also started on making a model of a building. In week two, I took the lead on making a design for the building and making the road in our game.

### Takeaway:

My exploration of p5.js not only introduced me to fundamental concepts in creative coding but also helped with  my problem-solving skills. By experimenting with code and tackling challenges, I gained a deeper understanding of how to bring my creative ideas to life through programming. This experience not only expanded my technical knowledge but also inspired me to continue exploring the endless possibilities of coding in the realm of art and interactive design. I also learned how to use keyIsDown(), fill() properly.

### Next Steps:

Continuing to experiment with p5.js and exploring its vast potential for creating interactive visualizations and artistic projects. Further practice will deepen my understanding and enable me to undertake more complex coding challenges.


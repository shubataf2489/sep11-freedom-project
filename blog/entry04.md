
# Entry 4
##### 03/18/24

### Process

My current stage in the Engineering Design Process (EDP) is building my project. A little recap of what my project is: a game that uses A-Frame. My partner and I aim to create a stress-relieving shooting game. We plan on making a 3D simulation of our game with stages featuring unique backgrounds. To learn my tool, I had to understand how A-Frame works and the components A-Frame uses. To get a better understanding of my tool (A-Frame), I read documentations made by the developer. Now, my partner and I use jsbin to code and test new things and when we like the code, we add it to our IDE.

Every weekend, my partner and I call each other and share our screen every time we code to show each other what we are doing. Calling each other makes us accountable to do the work. Each week we alternate on who leads. On week one, Shelly took the lead on selecting a background that will be best for our game and I listed the pros and cons of each setting. Shelly also started on making a model of a building. On week two, I took the lead on making a design for the building and making the road in our game.

### Content

[Link to code](../3d-site/index.html)

Currently, I think we are focusing on making a foundation for our games through HTML and starting next week, we will start coding for JavaScript more.

I have learned a lot of things while learning and coding using A-Frame.

My thought process and accomplishments made so far:
- How to make buildings have texture and designs.

Tip: Even if the text is really long, try to read it because it's really helpful.
- We include `<a-scene>` in the `<body>`. `<a-scene>` will contain every entity in our scene.
 `<a-scene>` handles all of the setup that is required for 3D: setting up WebGL, the canvas, camera, lights,

- A-Frame uses a right-handed coordinate system. With the default camera direction: positive X-axis extends right, positive Y-axis extends up, and the positive Z-axis extends out of the screen towards us.

- Decided the setting for our game level 1: Default

Disclaimer: These are all direct notes I found important from the documentation.
We decided that default would be best to add our own buildings on.

[Link to Creating Image Descriptors](https://aframe.io/blog/arjs3/)

### Recap:

My partner and I are using A-Frame to make a 3D simulation of a game. We want to create a shooting game that can help release pent-up stress from school, work, and etc. Our goal is to make a game that is interesting and relaxing. It may sound ironic that a shooting game can be relaxing, but all of the frustration and anger or stress can be let out through playing games. According to the article [How Do Video Games Reduce Stress?](https://www.healthygamer.gg/blog/do-video-games-reduce-stress#:~:text=When%20we%20play%20a%20video,the%20stresses%20of%20the%20day.), we are going to use games that have already been made through A-Frame to take inspiration and eventually make a game that has 360 images where you can move and interact with objects like cars, airplanes, and guns. We will be using A-Frame to create a 360-degree interactive game featuring moving and interactable items such as vehicles, aircraft, and firearms.

Some important things I found in the text:
- Location-based tracking uses real-world coordinates to place AR content in context. Users can move freely (outdoors for better precision), and content associated with their location will be scaled and placed accordingly (e.g.: content will render bigger/smaller based on the distance to the user).

- Replace `<add-your-latitude>` and `<add-your-longitude>` with your GPS coordinates. Get data from `latlong` to get data.

- Change the scale property according to the distance of the place you specified with the coordinates: if you are not seeing the text, try to scale it up or choose a place much nearer.

- We used the custom look-at A-Frame component, that makes the content always look towards the user camera. This is fundamental, in particular for 2D content as text.

- My partner and I worked together to discuss our next steps.
- My partner and I are on track and every weekend we call to make progress with our project.
- Last week we worked on setting a background and make a mini-demo of our final project.
- Before we had 2 buildings, some shapings in the back and a plain background.
- We wanted to make our building look 3D but realized it would be very time-consuming if we coded 10 buildings and made it realistic.
- Thus, when I was tinkering a few months back, I realized that I was able to make textured blocks.
- I went to Google and searched for "building texture".
- Then I copied the image URL.
- Thankfully it worked.
- Later on, we decided to make a road for our setting
- That was the hard part because whenever I changed the height, the line changed positions and there wasn't any pattern, so I had to constantly change the number of everything to see how to get the `<a-plane>` will be centered.
- I later made a yellow line to mirror a realistic road.

## Skills

- Communication: I had to communicate and collaborate and share my findings with my partner on many occasions to ensure we were on the same page. As I have mentioned before every weekend my partner and I call each other and share our screen every time we code to show each other what we are doing. Calling each other makes us accountable to do the work. Each week we alternate on who leads. On week one, Shelly took the lead on selecting a background that will be best for our game and I listed the pros and cons of each setting. Shelly also started on making a model of a building. On week two, I took the lead on making a design for the building and making the road in our game.

For example, on Mondays, we discussed what we worked on so far and split up all the components we think will help us with our project. My partner and I also share any resources like websites or videos that are useful.

- Time management: Since I can't work only on the project, I'm trying to split up my work throughout the day. On Mondays, I try to find new findings or tutorials to work on, and whenever I have the time, I work on them. On Saturdays, my partner and I call to work and make progress on our project. On Sundays, I reflect on what I learned and take note of the useful things I learned.

## Next steps:

- Making the game look realistic by adding characters, trees, cars, roads, target

- Learn geometry component to help make cars
- Also, we want to work on learning animation for making moving trees and a moving car.
Over the course of 2 weeks, my partner and I want to learn the components:
- Person (POV) - controls the camera/viewpoint
- Hand-controls - to help the player move the player’s movement
- Reflection - makes the characters stand out from the background by putting more light on top of them and adding a shadow.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)

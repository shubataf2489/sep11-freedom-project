
# Entry 4
##### 03/18/24

### Process

My current stage in the Engineering Design Process (EDP) is building my project. A little recap of what my project is: a game that uses A-Frame. My partner and I aim to create a stress-relieving shooting game. We plan on making a 3D simulation of our game with stages featuring unique backgrounds. To learn my tool, I had to understand how A-Frame works and the components A-Frame uses. To get a better understanding of my tool (A-Frame), I read documentations made by the developer. Now, my partner and I use jsbin to code and test new things and when we like the code, we add it to our IDE.

Every weekend, my partner and I call each other and share our screen every time we code to show each other what we are doing. Calling each other makes us accountable to do the work. Each week we alternate on who leads. On week one, Shelly took the lead on selecting a background that will be best for our game and I listed the pros and cons of each setting. Shelly also started on making a model of a building. In week two, I took the lead on making a design for the building and making the road in our game.

### Content

[Link to code](https://github.com/shubataf2489/3d-site/blob/main/index.html)

```html

<html>
  <head>
  <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  <script src="https://unpkg.com/aframe-environment-component/dist/aframe-environment-component.min.js"></script>
</head>
  <body>
    <a-scene>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9" animation="property: object3D.position.y; to: 2.2; dir: alternate; dur: 2000; loop: true"></a-box>></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
       <a-sphere position=".5 1.80 -4" radius=".2" color="#000000"></a-sphere>
      <a-sphere position="-.5 1.80 -4" radius=".2" color="#000000"></a-sphere>


      <a-cylinder src="https://i.imgur.com/mYmmbrp.jpg" position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-sky color="#ECECEC"></a-sky>
      <a-scene>
  <a-box src="https://i.imgur.com/mYmmbrp.jpg"color="red" position="0 2 -5" rotation="0 45 " scale="2 2 2"></a-box>
      <a-plane position="17 0.1 20" rotation="-90 6 80" width="10" height="60" color="#000000"></a-plane>
      <a-plane position="10 0.2 20" rotation="-90 6 80" width="1" height="50" color="#FFFF00"></a-plane>


        <a-entity environment="preset: ; dressingAmount: 500"></a-entity>

          <a-box src="data:image/jpeg;base64,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" position="-7 0 12" color="#FFFFFF" width="4" height="20" depth="4"></a-box>

           <a-box position="17 0 12" color="#C4A484" width="8" height="12" depth="8"></a-box>
</a-scene>
    </a-scene>
  </body>
</html>
```

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
- Last week we worked on setting a background and making a mini-demo of our final project.
- Before we had 2 buildings, some shapes in the back and a plain background.
- We wanted to make our building look 3D but realized it would be very time-consuming if we coded 10 buildings and made it realistic.
- Thus, when I was tinkering a few months back, I realized that I was able to make textured blocks.
- I went to Google and searched for "building texture".
- Then I copied the image URL.
- Thankfully it worked.
- Later on, we decided to make a road for our setting
- That was the hard part because whenever I changed the height, the line changed positions and there wasn't any pattern, so I had to constantly change the number of everything to see how to get the `<a-plane>` to be centered.
- I later made a yellow line to mirror a realistic road.

## Skills

- Communication: I had to communicate and collaborate and share my findings with my partner on many occasions to ensure we were on the same page. As I have mentioned before, every weekend my partner and I call each other and share our screen every time we code to show each other what we are doing. Calling each other makes us accountable to do the work. Each week we alternate on who leads. On week one, Shelly took the lead on selecting a background that will be best for our game and I listed the pros and cons of each setting. Shelly also started on making a model of a building. In week two, I took the lead on making a design for the building and making the road in our game.

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



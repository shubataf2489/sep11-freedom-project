
# Entry 3
##### 03/12/24

My current stage in the Engineering Design Process (EDP) is understanding and making a game plan for my game. A little recap of what my project is: a game that uses A-Frame. My partner and I aim to create a stress-relieving shooting game. We plan on making a 3D simulation of our game with stages featuring unique backgrounds. To learn my tool, I had to understand how A-Frame works and the components A-Frame uses. To get a better understanding of my tool (A-Frame), I read documentations made by the developer. I learned many interesting things, such as:
Although it is hard to find more resources that can teach me about how to use A-frame to make a shooting score or how to shoot. I plan on asking other people on the Aframe slack if they know/have ever made a game that keeps score through Aframe. If that doesn't work out as plan I will try to google for more resources.

* A-Frame is a JavaScript framework.

* A-Frame can be paired with other tools like Blender & three.js.
* I learned that I can control the viewer's viewpoint with a selector to `<a-asset-item>` or a URL to Supercraft JSON.

* Inspector tool to get a different view of the scene and see the visual effect of tweaking entities.

* The Inspector is similar to the browser’s DOM inspector but tailored for 3D and A-Frame. [Inspector tool](https://github.com/aframevr/aframe-inspect)

From following tutorials:

* I learned that I need to use `animation_up`, `animation_drive`, `animation_down` based on the animations I wanted.

* `includeEnvironment` - include environment (sky, ground, lights).
* `includeShadows` - can decide whether the mesh should receive and cast shadows.

* Although making a floating boat that seems like it's naturally going up and down is really complicated. The hardest thing to do is getting the timing right to make the boat go up and down.

Tutorials I followed:
- [tutorial on making 3d buildings](https://www.youtube.com/watch?v=5lTAt3HGPSw)

- [tutorial on making animation](https://www.youtube.com/watch?v=ZGk5XlPscsk)

- [link to an A-Frame tool](https://www.npmjs.com/package/aframe-supercraft-loader)

Learning all of these details helped me understand the fundamentals of A-Frame and gave me a better understanding of all the things I can do with A-Frame. I plan on doing things like:

 - have a sunset
 - moving text
 - moving objects
 - night turning into day
 - create a 3D building site using A-Frame.io and Blender.

## CONTENT:

 My partner and I are using A-Frame to make a 3D simulation of a game. We want to create a shooting game that can help release pent-up stress from school, work, and etc. Our goal is to make a game that is interesting and relaxing. It may sound ironic that a shooting game can be relaxing, but all of the frustration and anger or stress can be let out through playing games. According to the article [How Do Video Games Reduce Stress?](https://www.healthygamer.gg/blog/do-video-games-reduce-stress#:~:text=When%20we%20play%20a%20video,the%20stresses%20of%20the%20day.), we are going to use games that have already been made through A-Frame to take inspiration and eventually make a game that has 360 images where you can move and interact with objects like cars, airplanes, and guns. We will be using A-Frame to create a 360-degree interactive game featuring moving and interactable items such as vehicles, aircraft, and firearms.
While working on researching A-Frame, I came across a really interesting code:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Basic Scene with Environment - A-Frame</title>
    <meta name="description" content="Basic Scene with Environment - A-Frame">
    <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
    <script src="https://unpkg.com/aframe-environment-component@1.1.0/dist/aframe-environment-component.min.js"></script>
  </head>
  <body>
    <!-- Try changing the preset to one of default, contact, egypt, checkerboard, forest, goaland, yavapai, goldmine, 
         threetowers, poison, arches, tron, japan, dream, volcano, starry, osiris. -->
    <!-- See more environment options: https://github.com/feiss/aframe-environment-component#parameters -->
    <a-scene environment="preset: forest">
      <a-assets>
        <img id="boxTexture" src="https://i.imgur.com/mYmmbrp.jpg">
      </a-assets>
      
      <a-box
        src="#boxTexture"
        position="0 2 -5"
        rotation="0 45 45"
        scale="2 2 2"
        animation__position="property: object3D.position.y; to: 2.2; dir: alternate; dur: 2000; loop: true"
        animation__mouseenter="property: scale; to: 2.3 2.3 2.3; dur: 300; startEvents: mouseenter"
        animation__mouseleave="property: scale; to: 2 2 2; dur: 300; startEvents: mouseleave"></a-box>
      
      <a-entity text="value: Hello, A-Frame; color: #FAFAFA; width: 5; anchor: align" position="-0.9 0.2 -3" scale="1.5 1.5 1.5"></a-entity>
      <a-camera>
        <a-cursor color="#FAFAFA"></a-cursor>
      </a-camera>
    </a-scene>
  </body>
</html>
```

#### Mini project

Note: I worked on some mini-projects, but this one was the most recent project and I learned the most from this.

This made a dystopian world with boxes flying in a pattern.

When I saw this, I knew I had to make this one of the settings for the game.

The way I changed the code was, take a stater code provided by Aframe and make something interesting by combining both codes. 

```html
<html>
  <head>
  <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  <script src="https://unpkg.com/aframe-environment-component/dist/aframe-environment-component.min.js"></script>
</head>
  <body>
    <a-scene>
      <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"          animation="property: object3D.position.y; to: 2.2; dir: alternate; dur: 2000; loop: true"></a-box>
></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
       <a-sphere position=".5 1.80 -4" radius=".2" color="#000000"></a-sphere>
      <a-sphere position="-.5 1.80 -4" radius=".2" color="#000000"></a-sphere>

      
      <a-cylinder src="https://i.imgur.com/mYmmbrp.jpg" position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
      <a-sky color="#ECECEC"></a-sky>
      <a-scene>
  <a-box color="red" position="0 2 -5" rotation="0 45 " scale="2 2 2"></a-box>

  
        <a-entity environment="preset: forest; dressingAmount: 500"></a-entity>
       
</a-scene>
    </a-scene>
  </body>
</html>

```

## Next Steps:

I learned many components, and now I know which ones I will need to use and which ones I don't.

- I plan on learning the component material.

According to A-Frame: The material component gives appearance to an entity. We can define properties such as color, opacity, or texture. This is often paired with the geometry component, which provides shape.

This will help us a lot while making obstacles in the game.

- I also plan on learning the component `magicleap-controls`.

According to A-Frame: The `magicleap-controls` component interfaces with the Magic Leap controller. It wraps the tracked-controls component while adding button mappings, events, and Magic Leap controller model.

This will help us since we are planning on making levels in our game.

- I also plan on learning the component Text.

According to A-Frame: In 2D web development, text is the most basic thing because the browser’s renderer and layout engine handle everything. In a 3D context, we don’t have those luxuries. The text component renders signed distance field (SDF) font text.

Learning the component text will help us make texts move in the game, which is one of our goals.



## Skills

* Collaboration: My partner and I asked our peer (William) for help in debugging a code. In short, we were trying to make a small fan that can move its wings and didn’t realize that it can only be done if used three.js, but our peer helped us realize that, and we were able to find another mini project to work on.
* Communication: I had to communicate and collaborate and share my findings with my partner on many occasions to ensure we were on the same page. For example, on Mondays, we discussed what we worked on so far and split up all the components we think will help us with our project. My partner and I also share any resources like websites or videos that are useful.

* Time management: Since I can't work only on the project, I always try to do my project on Mondays and Tuesdays. On Mondays, I try to find new findings or tutorials to work on, and whenever I have the time, I work on them. On Sundays, I reflect on what I learned and take note of the useful things I learned.

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)

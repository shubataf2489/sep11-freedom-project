# Tool Learning Log

Tool:  Aframe

Project: Shooter game

---

11/10/21



Referring to the YouTube video https://youtu.be/cS8uGfd_oG8?si=ei0Qw-JAGN4aTQAm, I learned how to create a setting for my aircraft. I incorporated a blue sky, some clouds, and a bird, although the bird looks very 2D.Another skill I developed during tinkering is organization.

* This code    <a-scene countdown="start: 05:00; value: 00:00" gamestate="health: 5; wave: 0" gamestate-visuals="" decals="maxDecals: 30; src: #bulletDecal; size: 0.3" vr-analytics>
Is the way the user will first see the game setup, so there will be 5 lives and they will have 30 seconds to start shooting. This was something very important I learned because I can later use a code similar to this to make a shooting game.


One thing I realized while exploring the code is that
<!-- Hands. -->
   ```js  <a-entity id="leftHand" shoot-controls="hand: left" weapon shoot></a-entity>
     <a-entity id="rightHandPivot">
       <a-entity id="rightHand" shoot-controls="hand: right" weapon shoot></a-entity>
     </a-entity>


     <a-entity id="ring0" json-model="src:url(assets/models/ring.json); singleModel:true)" position="0 0 0" rotation="0 0 0" scale="1.3 1.3 1.3">
       <a-animation id="ring0anim" attribute="rotation" to="0 360 180" repeat="indefinite" dur="50000" easing="linear"></a-animation>
     </a-entity>


     <a-entity id="ring1" json-model="src:url(assets/models/ring.json); singleModel:true)" position="0 0 0" rotation="90 0 0">
       <a-animation id="ring anim" attribute="rotation" to="90 360 180" repeat="indefinite" dur="30000" easing="linear"></a-animation>
     </a-entity>


     <a-entity id="border" json-model="src:url(assets/models/border.json);" position="0 0 0"></a-entity>


     <a-entity id="highscores" position="2.2 2.2 -3.15" rotation="0 -45 0">
       <a-entity
         bmfont-text="fntImage:assets/fonts/mozillavr.png;
         fnt:assets/fonts/mozillavr.fnt;
         scale:0.002;
         text:HALL OF FAME;
         color:#f00">
         </a-entity>

```

The notes are always 1-5 words, it’s short and simple but clear. Moving forward I’m going to keep that in mind. Without even knowing much about the vocabulary that is used, I can already tell that this code is for the remote console that changes color when you shoot.


11/10/2023:

* I cloned the A -Frame (A-Blast) project and attempted to create different levels, a scoring system, and reduce the difficulty.
* I also aimed to change the background when the levels increases, but I found  identify the code for the background.
* After a few mistakes, I eventually located the code responsible for the background. Next I tried to makes a scoring system, but it didn't function as expected. I had difficulty figuring out how to add a score without the other parts of the code failing.
* Thus I couldn't  make the background change when the player went to the next  level, as I intended for the level transition to occur after the player successfully shot down 5 of the sprites.





11/17/2023-12/19/23

Followed the tutorial https://www.youtube.com/watch?v=y5SZCYT0Zwo

From the video I have learned how to:

I have learned how to:
* make the block color clear ( I have to use transparency and opacity)
* how to make the shape bend
* how to make the shape rotate
* I learned that the numbers need " " around them.
* Aframe aleady has many shapes that are saved in the site.
* codechanges- is very helpful to get/code new shapes && new colors
* I can also add new environments using codechanges.
* I looked at blogs and projects to understand other things I can do with a-frame.
* [One of the Blogs ](https://markpescecodex.com/we5/na.html)
* [Blogs ](https://aframe.io/blog/newsletter2/)
* The project that I have taken inspiration from is
* [Projects](https://www.kodub.com/apps/planetsbyearth)
* My partner Shelly and I had a disscustion about what we have been working on and what we should work on.
* In our discussion we decided that I will learn about the animation
* Shelly will learn the component laser-control.
* Shelly and I have decided that we want to make our freedom-project will look like.
* We will be focusing on tinkering with the components.
* I learned that A-Frame was built based on three. js, a JavaScript library that enables the creation of 3D content on the Web.
* while I was learning my component I stumbled upon reflextion
* I wanted to learn reflection
* Thus I remixed the started code that Aframe gave me and the code to enhance the reflextion of objects
* The code was
    ```js

    <a-scene reflection="directionalLight:a-light#dirlight;"></a-scene>
	<a-light id="dirlight" intensity="1" light="castShadow:true;type:directional" position="1 1 1"></a-light>
    
   ```
 * To my surprize the code didn't effect tne shapes at all.
 * I still intend to try it on my code later to see if it will change anything.
 * Some things I learned while learning about animations are:
 * boolean values where the to value will be applied at the end of the animation. Like property: visible; from: false; to: true; dur: 1.


     ```js <head>
    <meta charset="utf-8">
    <title>Animating on Events - A-Frame</title>
    <meta name="description" content="Hello, WebVR! • A-Frame">
    <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
    <script src="https://unpkg.com/aframe-environment-component@1.1.0/dist/aframe-environment-component.min.js"></script>
  </head>
  <body>
    <a-scene background="color: #FAFAFA" environment="preset: forest">
      <a-entity id="mouseCursor" cursor="rayOrigin: mouse" raycaster="objects: #box"></a-entity>
      
      <a-entity id="box" geometry="primitive: box" material="color: red" position="0 1.8 -3" rotation="0 30 0"
                animation__mouseenter="property: components.material.material.color; type: color; from: red; to: blue; startEvents: mouseenter; dur: 500"
                animation__mouseleave="property: components.material.material.color; type: color; from: blue; to: red; startEvents: mouseleave; dur: 500"
    </a-scene>
  </body> ```

  
* animation is really cool because you can change/ do many things like changing the color when you change the directions.


11/25/2023
 
Tinkering on replit
- all vr in aframe  starts with a dash
- Ex: <a-...>
- if you want to add attributes you have to put in the  <a-...>
- when adding an attributes put the thing then = then quotions and  number then ending quotation.
-  After a few mistakes, I eventually located the code responsible for the background. Next I tried to makes a scoring system, but it didn't function as expected. I had difficulty figuring out how to add a score without the other parts of the code failing.
- Thus I couldn't  make the background change when the player went to the next  level, as I intended for the level transition to occur after the player successfully shot down 5 of the sprites.
- Ex: <a-box color="cyan">
- By default the postion is always " 0 0 0"
- you can change the postion by typing  <a-plane color="cyan" width="4" height="4" rotation="-90 0 0" postion="0 0 -4">

-number 1= right
-number 2= left
-number 3= distance
-radius="1.25"
* Radius sets the size
* the bigger the num the bigger the shape
* You need color or else it's going to be white and you won't be able to see anything.
  
 ```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title> Tinkering with VR</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
  <script src="https://aframe.io/releases/1.4.0/aframe.min.js"></script>
  
</head>

<body>

  <a-scene> 

    <a-plane color="cyan" width="4" height="4" rotation="-90 0 0" position="0 0 -4"></a-plane>
<a-box color="purple" position="-1 0.5 -2" rotation="0 45 0" ></a-box>
      <a-sphere position="0 1.24 -5" radius="-1.25" color="pink"></a-sphere>
    <a-cylinder position="1 0.75 -3" radius="0.5" height="2" color="blue"></a-cylinder>
  </a-scene>
</body>

</html>
 ```
Use <a-entity> to create entities within the scene. Entities are the building blocks of your VR world.

Primitive Elements:
A-Frame provides primitive elements like <a-box>, <a-sphere>, <a-cylinder>, etc., to easily create basic shapes in your scene.


Components:
Components are attributes that define the appearance, behavior, or functionality of entities. Use them to add interactivity, animations, and more.


Animations:
A-Frame supports animations to bring your VR scene to life. Use the <a-animation> element or the animation component on entities.


Place a camera (<a-camera>) within your scene to define the viewpoint for users.


#### Jan 8,2023
 * I learned about different components.
 * I disscused with my partner about our next steps
 * we liked the component laser
 * We want to use laser in our project hopefully.
* Like the envMap and sphericalEnvMap properties define what environment the material reflects. The clarity of the environment reflection depends on the metalness, and roughness properties.
*There are things like video loops
* the video texture loops or autoplays depends on the video element used to create the texture. If we simply pass a URL instead of creating and passing a video element, then the texture will loop and autoplay by default. To specify otherwise, create a video element in the asset management system, and pass a selector for the id attribute (e.g., #my-video):
* I wanted to use Transparency to for the indows of the aircafts and front views but I learned that:
*" Transparency and alpha channels are tricky in 3D graphics. If you are having issues where transparent materials in the foreground do not composite correctly over materials in the background, the issues are probably due to underlying design of the OpenGL compositor (which WebGL is an API for)."
* But In an ideal scenario, transparency in A-Frame would “just work”.
*The sphericalEnvMap property takes a single spherical mapped texture. Of the kind you would assign to a <a-sky>.
* We can use a <canvas> as a texture source.
*Unlike textures, the envMap property takes a cubemap, six images put together to form a cube. The cubemap wraps around the mesh and applied as a texture.
<!--
This script places a badge on your repl's full-browser view back to your repl's cover
page. Try various colors for the theme: dark, light, red, orange, yellow, lime, green,
teal, blue, blurple, magenta, pink!
-->

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next

-->



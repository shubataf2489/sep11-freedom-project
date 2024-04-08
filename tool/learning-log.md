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
  </body>
  ```


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


01/16/2024


Some measures that A-Frame takes to minimize overhead include:

-the <iframe> will not display in VR nor can it integrate with the scene.

Making setAttribute synchronous with a reduced code path. Modifying an entity’s position via setAttribute('position', {x: 1, y: 2, z: 3}) almost directly touches the underlying three.js objects.

The overhead involves comparing new data to old data to determine whether a change needs to be triggered and invoking lifecycle handlers.

This makes most operations done in memory, a tiny bit similar to Virtual DOM.

Keeping everythingunder a single requestAnimationFrame and letting components hook into a single global render loop via the tick handler.

-talk to Shelly about what I learned

- Shelly and I agreed to make a demo of our project next week to know what we want to learn about next week.

- Shelly and I had a disagreement about what we want our next plans to be

- shelly want to continue learning new componenets

- I want to make a demo so we know which componenet will be useful for us to learn.

- shelly and came to the agreement that after this week we will learn how to make a small demo of how we want our project to look like, like a wire frame.

-A-Frame is a JavaScript framework.

for aframe you need to use techniques used in the 3D and game industry (e.g., geometry instancing, level-of-detail, object pooling.

### 01/22/2024

I'm following the [tutorial on making 3d buildings](https://www.youtube.com/watch?v=5lTAt3HGPSw)

Unfortunately my partner and I became busy with other schoolwork and were able to dedicate our time into making a demo of our project.

In the video I what I learned from the code really interested me because it seems complicated but it only takes 90 sec to do if you learn/undertsand that concept.

In the video, the youtuber shows how I created a 3D buildings site using Aframe.io and Blender.

In the video the youtuber teaches things like exporting a .glb file, import it into an A-frame project, and adjust the camera and environment lighting.

My partner and I decided to make the demo next term and start fresh.

[tutorial on making animation](https://www.youtube.com/watch?v=ZGk5XlPscsk)
I learned how to make cars move automatic using aframe.

It is wayy more easier than I thought it would be to code animations.


### 02/05/2024

I learned that I need to use animation_up, animation_drive , animation_down based on what animations I wanted.

Although maing a floating boat that seems like it's naturally is going up and down is really complicated. The hardest thing to do is getting the timing right to make the boat go up and down.

I also learned how to make the boat seem a though it is tiliting left and right.

To make an order you can use timeline to pick a order that is doing 2 animation at the same time and choose which animation should be first and last.


From this video I was thing I can make it seem as though there is wind flowing through the trees when the aircraft is used.

I shared my resources with my partner

I recommended my partner which tutorials to follow

### 02/25/2024

I learned what a [link to an aframe tool](https://www.npmjs.com/package/aframe-supercraft-loader) is helpful then making a 3d world.

Things I learned on the website:

includeEnvironment-  include environment (sky, ground, lights).

includeShadows- can decide whether the mesh should receive and cast shadows.

I learned that I can control the viewer's view point  with selector to <a-asset-item> or URL to Supercraft JSON.

Inspector tool to get a different view of the scene and see the visual effect of tweaking entities.

The Inspector is similar to the browser’s DOM inspector but tailored for 3D and A-Frame. (Inspecter tool)(https://github.com/aframevr/aframe-inspector)

To modify the material of a model, we need to wait for the model to load, and then modify the three.js meshes created from the mode

Sometimes textures just won’t work right off the bat. This is usually because exporters use absolute paths like C:\\Path\To\Model\texture.jpg or /Path/To/Model/texture.jpg

I helped my partner understand what code she should try doing and practicing more with through a yellkey.


### 03/04/2024

* Learning how to set up a frame componet from scratch
[Link to Building a Basic Scene](https://aframe.io/docs/1.5.0/guides/building-a-basic-scene.html)
[Link to learning aframe html](https://aframe.io/docs/1.5.0/introduction/html-and-primitives.html)
* Tip: Even if the text is really long try to read it because it's really helpful.
-  we include <a-scene> in the <body>. <a-scene> will contain every entity in our scene.
 <a-scene> handles all of the setup that is required for 3D: setting up WebGL, the canvas, camera, lights,

- Frame uses a right-handed coordinate system. With the default camera direction: positive X-axis extends right, positive Y-axis extends up, and the positive Z-axis extends out of the screen towards us:

- decided the setting for our game level 1: Default

 Disclaimer: These are all direct notes I found important from the documentation.

// Everything combined

```HTML

 <html>
  <head>
  <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  <script src="https://unpkg.com/aframe-environment-component/dist/aframe-environment-component.min.js"></script>
</head>
  <body>
    <a-scene>
<a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9" animation="property: object3D.position.y; to: 2.2; dir: alternate; dur: 2000; loop: true"></a-box>></a-box>// has texture
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
       <a-sphere position=".5 1.80 -4" radius=".2" color="#000000"></a-sphere>
      <a-sphere position="-.5 1.80 -4" radius=".2" color="#000000"></a-sphere>


      <a-cylinder src="https://i.imgur.com/mYmmbrp.jpg" position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-sky color="#ECECEC"></a-sky>
      <a-scene>
  <a-box color="red" position="0 2 -5" rotation="0 45 " scale="2 2 2"></a-box>


        <a-entity environment="preset: default; dressingAmount: 500"></a-entity>// the setting



</a-scene>
    </a-scene>
  </body>
</html>
```
It took shelly and me an hour to decide what setting would fit our game best and after many discussions, we decided that defalt would be best to add our own buildings on.

[Link to Creating Image Descriptors](https://aframe.io/blog/arjs3/)



Some important things I found in the text:

* Location-based tracking uses real-world coordinates to place AR content in context. Users can move freely (outdoors for better precision) and content associated with their location will be scaled and placed accordingly (e.g: content will render bigger / smaller based on distance to the user).

* Replace <add-your-latitude> and <add-your-longitude> with your GPS coordinates. Gte data from `latlong` to get data.

* Change the scale property according to the distance of the place you specified with the coordinates: if you are not seeing the text, try to scale it up or choose a place much near.

* We used the custom look-at A-Frame component, that makes the content always look towards the user camera. This is fundamental, in particular for 2D content as text.

03/10/2024

* My partner and I worked together to discuss our next steps.
* My partner and I are on track and every weekend we call to make progess with our porject.
* last week we worked on setting a background and make a mini demo of our final project.
* Before we had 2 buildings, some shapings in the back and a plain background.
* We wanted to make out building look 3d but realized it would be every time consuming if we coded 10 building and made it realistic.
* Thus, When I was tinkering a few months back, I realized that I was able to make textured blocks.
* I went to google and searched for "building texture".
* Then I copied the image url.
* Thankfully it worked.
* Later on we decided to make a road for our setting
* that was the hard oart because when ever I changed the height, the line changed postions and their wasn't any pattern, so I had to constantly change the number of everything to see how to get the `<a-plane>`  will be centered.
* I later made a yellow line to mirror a realistic road.
```js
 <a-box src="data:image/jpeg;base64,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" position="-7 0 12" color="#FFFFFF" width="4" height="20" depth="4"></a-box>
```
This is the coded that made my rectangular prism look similar  to a building.


### 03/24/2024

* The main thing I focused on this week was making making a city.
* I downloaded many building textures.
* I made many build blocks with different sizes and shapes
* This gave the illusion of a realistic city.
* I also didn't make the buidlings aligned with each other
* I some placed them in the back and some in the front to make the city look more realistic.
* A lot fo them didn't look, so I had to delete them.
* I had trial and see if the buidling texture would duit the aesthetic.
* The ones that did look good I saved them.
* This process took me a while to do
* While I worked on the Buildings, my partner focused on maing the car layout


### 03/31/2024
* My partner and I decided to do call to discuss the nest steps as we are almost done with the setting.
* We need to figure out the shooting side of the game to be able to finish the setting.
* Figuring out a way to create a shooting game in Aframe was a big challenge.
* I had to watch many videos and thankfull some people have created a shooting game using Aframe.
* The problem was the website that has the explicit explanation on how to code a shooting game is down.
*  My partner and I are in hopes that the website gets back up but if not we are on the journey to find other videos to teach us.
* These are some of the tutorials that I found useful:
* (Tutorial 1) [https://supermedium.com/aframe-super-shooter-kit/examples/supercraft/]
* (Tutorial 2) [https://www.youtube.com/watch?v=q3bjSDTgUAg]
* (Tutorial 3 ) [https://www.youtube.com/watch?v=SeV7RmjxfTY]
* (Tutorial 4 ) [https://github.com/supermedium/aframe-super-shooter-kit]
* (Tutorial 5 ) [https://www.youtube.com/watch?v=t5Hou5QsRiE]
     ### Terms:
* damagePoints -How many health points to remove from target when hitting target.
* maxTime-Life time of bullet in seconds. When elapsed, the bullet will be removed.
* poolSize -How many copies of this bullet can be on screen at once.
* speed- Speed of bullet in meters per second.
* hit	Target was hit by a bullet.
* die	Target ran out of healthPoints and has been destroyed.

### 04/08/2024


1. **A-Frame Setup**: 
   - The HTML file sets up an A-Frame scene using `<a-scene>`.
   - A-Frame framework and A-Frame GUI component are included via script tags.
  
2. **Camera and Controls**:
   - The camera entity is created using `<a-entity camera>`.
   - `look-controls` and `wasd-controls` components are added for mouse-based look and WASD movement.

3. **Gun Representation**:
   - The gun is represented by a gray box with `<a-entity>` tag.
   - Its position, scale, and color are defined using `position`, `scale`, and `material` attributes.

4. **Targets**:
   - Two target entities are created with the class `.target`.
   - They are represented by colored boxes (`<a-entity>`) positioned in the scene.
   - Each target's position, scale, and color are defined using attributes.

5. **GUI Button**:
   - A GUI button is created using `<a-gui-button>` tag.
   - It's positioned in front of the camera using `position` attribute.
   - When clicked (`onmouseup` event), the `shoot()` function is triggered.

6. **JavaScript Function `shoot()`**:
   - This function is triggered when the shoot button is clicked.
   - It finds all elements with the class `.target`.
   - It iterates through each target and calculates the distance between the gun and the target.
   - If the distance is less than a threshold (in this case, 2 units), the target is removed from the scene (`removeChild()`).


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



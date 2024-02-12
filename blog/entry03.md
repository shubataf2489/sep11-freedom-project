# Entry 3
##### 03/12/24

My current stage in the Engineering Design Process (EDP) is understanding making a game plan for my game. A little recap of what my project is a game that uses Aframe. My patrner and I aim to make a stress realiving, shooting game. We plan on making a 3d simualtion of our game and have stages with unique backgrounds. To learn my tool I had to learn how Aframe works and the components Aframe uses.  To get better understanding of my tool (Aframe). I read documentations made by the developer. I learn many interesting likes such as:

* A-frame is a JavaScript framework

* A-frame can be paired with other tools like Blander & three.js
* I learned that I can control the viewer's view point  with selector to <a-asset-item> or URL to Supercraft JSON.

* Inspector tool to get a different view of the scene and see the visual effect of tweaking entities.

* The Inspector is similar to the browser’s DOM inspector but tailored for 3D and A-Frame. (Inspecter tool](https://github.com/aframevr/aframe-inspect
From following tutorials:

* I learned that I need to use animation_up, animation_drive , animation_down based on what animations I wanted.

* includeEnvironment-  include environment (sky, ground, lights).

* includeShadows- can decide whether the mesh should receive and cast shadows.

* Although maing a floating boat that seems like it's naturally is going up and down is really complicated. The hardest thing to do is getting the timing right to make the boat go up and down.

Tutorials I followed:
- [tutorial on making 3d buildings](https://www.youtube.com/watch?v=5lTAt3HGPSw)

- [tutorial on making animation](https://www.youtube.com/watch?v=ZGk5XlPscsk)

- [link toan aframe tool](https://www.npmjs.com/package/aframe-supercraft-loader)



 Learning all of these detail helped me understand the fundamental of Aframe and see gave me a better undertsandngof all of the things I can do with Aframe. I plan on doing things like:

 - have a sunset
 - moving text
 - moving objects
 - night turning into day
 - created a 3D buildings site using Aframe.io and Blender.

 These are some of the examples I have seen other aframe users create and it intrigued me.




 While working on researching about Aframe I came across a really interesting code

 ```HTML
 <!DOCTYPE html>
<html>
  <head>
    <script src="https://aframe.io/releases/0.8.2/aframe.min.js"></script>
    <script src="play-all-model-animations.js"></script>
    <script>
      AFRAME.registerComponent('modify-materials', {
        init: function () {
          // Wait for model to load.
          this.el.addEventListener('model-loaded', () => {
            // Grab the mesh / scene.
            const obj = this.el.getObject3D('mesh');
            // Go over the submeshes and modify materials we want.
            obj.traverse(node => {
              if (node.name.indexOf('ship') !== -1) {
                node.material.color.set('red');
              }
            });
          });
        }
      });
    </script>
  </head>
  <body>
    <a-scene background="color: #ECECEC">
      <a-assets>
        <a-asset-item id="cityModel" src="https://cdn.aframe.io/test-models/models/glTF-2.0/virtualcity/VC.gltf"></a-asset-item>
      </a-assets>
      <a-entity gltf-model="#cityModel" play-all-model-animations modify-materials></a-entity>
    </a-scene>
  </body>
</html>
```

#### Mini project

Note: I worked on some mini projects but this one was the is the most recent project and I learned the most from this.

This made a dystopian world with boxs flying in a pattern

when I saw this I knew I had to make this one of the settings for the game.


The way I changed the code was instead of flying boxes there were flying airplanes and the setting was the game but I changed the background because I really liked tha dystopian setting. I also stopped the flying boxes

```HTML
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A-Frame VR Scene with Airplanes</title>
    <script src="https://aframe.io/releases/0.8.2/aframe.min.js"></script>
    <script src="play-all-model-animations.js"></script>
    <script>
      AFRAME.registerComponent('modify-materials', {
        init: function () {
          // Wait for model to load.
          this.el.addEventListener('model-loaded', () => {
            // Grab the mesh / scene.
            const obj = this.el.getObject3D('mesh');
            // Go over the submeshes and modify materials we want.
            obj.traverse(node => {
              if (node.name.indexOf('ship') !== -1) {
                node.material.color.set('red');
              }
            });
          });
        }
      });
    </script>
  </head>
  <body>
    <a-scene background="color: #ECECEC">
      <a-assets>
        <a-asset-item id="cityModel" src="https://cdn.aframe.io/test-models/models/glTF-2.0/virtualcity/VC.gltf"></a-asset-item>
        <a-asset-item id="airplaneModel" src="plane.jpeg"></a-asset-item>
      </a-assets>

      <!-- City Model with Animations and Modified Materials -->
      <a-entity gltf-model="#cityModel" play-all-model-animations modify-materials></a-entity>

      <!-- Airplane Model -->
      <a-entity gltf-model="#airplaneModel" position="0 2 -5" rotation="0 180 0" scale="0.5 0.5 0.5"></a-entity>

    </a-scene>
  </body>
</html>

```


## Next Steps:

I learned many components and now I know which ones I will need to use and which one I don't.

- I plan on learning the component material.

According to Aframe: The material component gives appearance to an entity. We can define properties such as color, opacity, or texture. This is often paired with the geometry component which provides shape.

This will help us a lot while making obstacles in the game

magicleap-controls

- I also plan on learning the component magicleap-controls.

According to Afreme: The magicleap-controls component interfaces with the Magic Leap controller. It wraps the tracked-controls component while adding button mappings, events, and Magic Leap controller model.

This will help us since we are planing on makeing levels in our game.

I also plan on learning the component Text.

According to Aframe:In 2D web development, text is the most basic thing because the browser’s renderer and layout engine handle everything. In a 3D context, we don’t have those luxuries. The text component renders signed distance field (SDF) font text.

Learning the component text will help us make texts move in the game, which is one of our goals.


## CONTENT:

 My partner and I are using a frame to make a 3d simulation of a game. We want to make a shoot game that can help realse pent up stress from school and work and etc. Our goal is to make a game that is interesting and relaxing. It may sound ironic that a shooting game can be relaxing but all of the frustration and anger or stress can be let out through playing games. According to the article (How Do Video Games Reduce Stress?)[https://www.healthygamer.gg/blog/do-video-games-reduce-stress#:~:text=When%20we%20play%20a%20video,the%20stresses%20of%20the%20day.] We are going to use games that have already been made through A Frame to take inspiration and eventually make a game that has 360 images where you can move and interact with objects like cars, airplanes and guns.  We will be using A-frame to create a 360-degree interactive game featuring moving and interactable items such as vehicles, aircraft, and firearms.



## Skills

* Collaboration: My partner and I asked our peer ( William), what he to help us debug a code. In short we were trying to make a small fan that can move it's wings and didn’t realize that it can only be done if use used three.js
but our helped us realize that and we were able to find another mini project to work on.
* Communication: I had to communicate and collaborate and share my finds with my partner on many occasions to ensure we were on the same page. For example, on mondays we discussed what we worked on so far and split up all the components we think will help us with our project. My partner and I also share any reaosuces like website or video that is useful.

* Time management: Since I can't work on only on theproject I always try to do my project on Mondays and and  Tuesdays. On mondays I try to find new findings or tutorial to work on and whenever I have the time I work on them. On sundays I reflect on what I learned and take a note of the usful things I learned.




[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)



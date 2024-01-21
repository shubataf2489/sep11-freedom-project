# Entry 2
#### 11/17/2023


Engineering Design Process:




My current stage in the Engineering Design Process (EDP) is still to better understand my tool and how to utilize it. To better understand my tool I have been reading other people's projects, they were made with an A-frame and their process. I have also been following tutorials  and exploring other projects for ideas. My next step is learning the components are shadow, pool, layers and light.  After that my partner and I plane to make a demo model of our project to see which skilll will be useful to learn.



As I have mentioned I cloned the A-Blast project into my IDE after I have done the tinkering with A-Blast I have moved on to other methods. [Tutorial ](https://www.youtube.com/watch?v=y5SZCYT0Zwo)






In the blogs people talk about their projects and in some they show the project, in others they talk about their process and struggles. My personal favorite story is because I want to make something similar to it
[One of the Blogs ](https://markpescecodex.com/we5/na.html)
[Blogs ](https://aframe.io/blog/newsletter2/)


The project that I have taken inspiration from is
[Projects](https://www.kodub.com/apps/planetsbyearth)
This project was really interesting to watch but the animation was very slow. In my project I will be focusing on not making animation slow and having a setting related to a starry-night.


I have learned how to:
* make the block color clear ( I have to use transparency and opacity)
* how to make the shape bend
* how to make the shape rotate
* I learned that the numbers need " " around them.
* Aframe already has many shapes that are saved in the site.
* code changes- is very helpful to get/code new shapes && new colors
* I can also add new environments using code changes.


Through the video I have gotten many insights on how to code on a frame. The more I learned through the video the more excited I felt to learn about it. The video helped me understand how I am going to make an aircraft and make the setting a night setting but I want to be able to change the setting from night to day, that's my future goal.








![](car.png)


#### Results
![](zoom.png)


#### mid-step


![](code.png)


#### Code


## Content/Goal:


My partner and I are using a-frame  because we want to make a video game that is pleasing to the eye, while being entertaining. My  goal is the same as before, it is to make a game that is both entertaining and calming. Ironically, playing a shooting game could help you relieve stress and release all of your frustrations, rage, and tension. The article "Do Video Games Reduce Stress?" claims as much. Using existing A Frame games as a model, we will eventually create a 360-degree interactive game featuring moving and interactable items such as vehicles, aircraft, and firearms. I've made the decision to use A-Frame to construct a flying obstacle game. I performed a number of tasks to test my tool. To better understand how aframe works I made a stater code from scratch to understand what does does what and why it does what. 

```js
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

   <a-plane color="cyan" width="4" height="8" rotation="-90 0 0" position="0 0 -4"></a-plane>
   <a-box color="purple" position="-1 0.5 -2" rotation="0 45 0" ></a-box>
   <a-sphere position="0 1.24 -5" radius="-1.25" color="pink"></a-sphere>
   <a-cylinder position="1 0.75 -3" radius="0.5" height="2" color="blue"></a-cylinder>
 </a-scene>
</body>
</html>
```
FRom making my own stater code I learned the following:

* all vr in aframe starts with a dash
  
Ex: <a-...>

* If you want to add attributes you have to put in the <a-...>
  
* When adding an attributes put the thing then = then quotions and number then ending quotation.
  
* After a few mistakes, I eventually located the code responsible for the background. Next I tried to makes a scoring system, but it didn't function as expected. I had difficulty figuring out how to add a score without the other parts of the code failing.
  
* Thus I couldn't make the background change when the player went to the next level, as I intended for the level transition to occur after the player successfully shot down 5 of the sprites.
  
* Ex:
  By default the postion is always " 0 0 0"
  
* you can change the postion by typing
  
-number 1= right -number 2= left -number 3= distance -radius="1.25"

* Radius sets the size
* the bigger the num the bigger the shape
* You need color or else it's going to be white and you won't be able to see anything.

* Use to create entities within the scene. Entities are the building blocks of your VR world.

* Primitive Elements: A-Frame provides primitive elements like , , , etc., to easily create basic shapes in your scene.

* Components: Components are attributes that define the appearance, behavior, or functionality of entities. Use them to add interactivity, animations, and more.

* Animations: A-Frame supports animations to bring your VR scene to life. Use the element or the animation component on entities.

* Place a camera () within your scene to define the viewpoint for users.



## skill
Organization: I had to organize my code so it was clear. Organizing the code was really important because I was learning something new. Organization was important for me to undertsand what each code did and if I had a bug. The main thing I focused on was indexation to organize my code better. 

Research/Growth mindset: I had to incorporate a growth mindset because I would have to research a lot and for that I would need patience to able able to research. Following through the tutorial was also a hassle because there were many new things I learned at the same time.




[Previous](entry01.md) | [Next](entry03.md)


[Home](../README.md)




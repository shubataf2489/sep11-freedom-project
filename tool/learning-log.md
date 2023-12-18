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





11/17/2023

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









<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next

-->



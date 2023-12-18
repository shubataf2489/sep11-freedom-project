# Entry 1
##### 11/13/21

My current stage in the Engineering Design Process (EDP) is understanding my tool and how to utilize it. I have decided to create a flying obstacle game using A-Frame. To experiment with my tool, I undertook various tasks.

Firstly, I cloned the A-Blast project https://github.com/aframevr/a-blast and attempted to create different levels, implement a scoring system, and reduce the difficulty. One skill I honed during tinkering is debugging, where I had to identify the bug causing my code to stop working. Additionally, I aimed to change the background during level transitions, but I faced challenges in identifying the relevant code for the background. After a few mistakes, I eventually located the code responsible for the background.I also tried to implement a scoring system, but it didn't function as expected. I struggled with figuring out how to add a score without interfering with other parts of the code. This hindered my ability to make the background change when the player advanced to the next level, as I intended for the level transition to occur after the player successfully shot down 5 of the sprites. When I cloned the A-Blast project https://github.com/aframevr/a-blast, I faced so many difficulties and the more I tried to unveil each topic the more it felt as if I was going down a rabbit hole. There was more than 20 directories


While tinkering with my tool, I reconsidered the shooting game idea and decided to create a game where a plane flies in the air. Using the up, down, left, and right arrows, I can control the airplane. I added obstacles to make the game challenging. Referring to the YouTube video https://youtu.be/cS8uGfd_oG8?si=ei0Qw-JAGN4aTQAm, I learned how to create a setting for my aircraft. I incorporated a blue sky, some clouds, and a bird, although the bird looks very 2D.Another skill I developed during tinkering is organization. When I cloned A-Blast, I had many files in my IDE, and I organized them by moving them into a separate folder outside of my JS to avoid confusion.


 Understanding the code was difficult but I managed to understand how the code worked.

“
 if (anchor === 'left') x = 0
        else if (anchor === 'right') x = -layout.width
        else if (anchor === 'center') x = -layout.width / 2
        else throw new TypeError('invalid anchor ' + anchor)


        // anchors text to top/center/bottom
        if (baseline === 'bottom') y = 0
        else if (baseline === 'top') y = -layout.height + layout.ascender
        else if (baseline === 'center') y = -layout.height / 2
        else throw new TypeError('invalid baseline ' + baseline)


        this.mesh.position.x = scale * x
        this.mesh.position.y = scale * y
        this.geometry.computeBoundingSphere()
      },


“
This code allows the user to maneuver the mouse in any way they want.

This code    <a-scene countdown="start: 05:00; value: 00:00" gamestate="health: 5; wave: 0" gamestate-visuals="" decals="maxDecals: 30; src: #bulletDecal; size: 0.3" vr-analytics>
Is the way the user will first see the game setup, so there will be 5 lives and they will have 30 seconds to start shooting. This was something very important I learned because I can later use a code similar to this to make a shooting game.


One thing I realized while exploring the code is that
<!-- Hands. -->
     <a-entity id="leftHand" shoot-controls="hand: left" weapon shoot></a-entity>
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
The notes are always 1-5 words, it’s short and simple but clear. Moving forward I’m going to keep that in mind. Without even knowing much about the vocabulary that is used, I can already tell that this code is for the remote console that changes color when you shoot.




CONTENT:
The reason me and my partner are using a frame is because we want to make a video game that is pleasing to the eye, while being entertaining. Our goal is to make a game that is interesting and relaxing. It may sound ironic that a shooting game can be relaxing but all of the frustration and anger or stress can be let out through playing games. According to the article Do Video Games Reduce Stress? We are going to use games that have already been made through A Frame to take inspiration and eventually make a game that has 360 images where you can move and interact with objects like cars, airplanes and guns.

Sources:
* https://github.com/aframevr/a-blast
* https://youtu.be/cS8uGfd_oG8?si=ei0Qw-JAGN4aTQAm


[Next](entry02.md)

[Home](../README.md)



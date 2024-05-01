
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


        <a-entity environment="preset: default; dressingAmount: 500"></a-entity>

         <a-box src="first-building.jpeg" position="-7 0 12" color="#FFFFFF" width="4" height="20" depth="4"></a-box>
           <a-box position="17 0 12" color="#C4A484" width="8" height="12" depth="8"></a-box>


    </a-scene>
  </body>
</html>

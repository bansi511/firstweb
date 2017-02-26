# firstweb

<!DOCTYPE html>
<!-- By Ada Rose Edwards @lady_ada_king. -->
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>A-Frame 80s</title>
    <meta name="description" content="Vaporwave aesthetic text By Ada Rose Edwards.">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:site" content="@lady_ada_king">
    <meta name="twitter:title" content="VR Vaporwa(v|r)e">
    <meta name="twitter:description" content="What is vaporwave? According to commenters in various music forums, it's 'chillwave for Marxists,' 'post-elevator music,' 'corporate smooth jazz Windows 95 pop,'">
    <meta name="twitter:image" content="http://i.imgur.com/B84J9uG.jpg">
    <meta property="og:image" content="https://raw.githubusercontent.com/ngokevin/kframe/master/components/text/examples/vaporwave/preview.jpg"></meta>
    <script src="https://rawgit.com/aframevr/aframe/917c06889ee1f3f79b7b1bbd9eab9815f9512503/dist/aframe.min.js"></script>
    <script src="../build.js"></script>
    <script src="https://cdn.rawgit.com/AdaRoseEdwards/facetype-fonts-for-a-frame/master/Dawning-of-a-New-Day_Regular.js"></script>
    <script src="https://cdn.rawgit.com/AdaRoseEdwards/facetype-fonts-for-a-frame/master/Exo%202%20Black_Regular.js"></script>
    <script src="https://cdn.rawgit.com/AdaRoseEdwards/facetype-fonts-for-a-frame/master/Exo%202_Bold%20Italic.js"></script>
  </head>
  <body>
    <a-scene inspector="url: https://aframe.io/aframe-inspector/dist/aframe-inspector.min.js">
      <a-assets>
        <img id="pink" src="https://img.gs/bbdkhfbzkk/stretch/http://i.imgur.com/1hyyIUi.jpg" crossorigin="anonymous" />
        <img src="https://img.gs/bbdkhfbzkk/stretch/https://i.imgur.com/25P1geh.png" id="grid" crossorigin="anonymous">
        <img src="https://img.gs/bbdkhfbzkk/2048x1024,stretch/http://i.imgur.com/WMNH2OF.jpg" id="chrome" crossorigin="anonymous">
        <img id="sky" src="https://img.gs/bbdkhfbzkk/2048x2048,stretch/http://i.imgur.com/WqlqEkq.jpg" crossorigin="anonymous" />
      </a-assets>

      <a-entity scale="2 2 2" geometry="primitive: torusKnot;" position="0 6 -10" material="color: magenta; metalness:1; roughness: 0.1; sphericalEnvMap: #sky;">
        <a-animation easing="linear" attribute="rotation" dur="10000" to="0 0 360" repeat="indefinite"></a-animation>
      </a-entity>

      <a-entity position="-3 1 -6" rotation="5 0 0">
        <a-entity
          rotation="0 0 5"
          position="0 2 0.2"
          text="text: Virtual Reality; font:dawning of a new day; bevelEnabled: true; bevelSize: 0.05; bevelThickness: 0.05; curveSegments: 12; size: 1; height: 0;"
          material="color:lavenderblush; metalness:1; roughness: 0; sphericalEnvMap: #pink;"
        ></a-entity>

        <a-entity position="-0.5 0.5 -0.5" scale="0.6 1.2 1" text="text: VAPORWAVE; font: exo 2 black; bevelEnabled: true; bevelSize: 0.1; bevelThickness: 0.1; curveSegments: 1; size: 1.5; height: 0.5;" material="color:pink; metalness:0.9; roughness: 0.05; sphericalEnvMap: #chrome;"></a-entity>

        <a-entity position="1 0 0.3" text="text: Aesthetic; font: exo 2;  style: italic; size: 0.8; weight: bold; height: 0;" material="shader: flat; color:white;"></a-entity>
        <a-entity position="1 0 0.3" text="text: Aesthetic; font: exo 2;  style: italic; size: 0.8; weight: bold; height: 0; bevelEnabled: true; bevelSize: 0.04; bevelThickness: 0.04; curveSegments: 1;" material="shader: flat; color:white;transparent: true; opacity: 0.4;"></a-entity>
      </a-entity>

      <a-entity position="0 0 0"
        geometry="primitive: plane; width: 10000; height: 10000;" rotation="-90 0 0"
        material="src: #grid; repeat: 10000 10000; transparent: true;metalness:0.6; roughness: 0.4; sphericalEnvMap: #sky;"></a-entity>

      <a-entity light="color: #ccccff; intensity: 1; type: ambient;" visible=""></a-entity>
      <a-entity light="color: ffaaff; intensity: 1.5" position="5 5 5"></a-entity>
      <a-entity light="color: white; intensity: 0.5" position="-5 5 15"></a-entity>
      <a-entity light="color: white; type: ambient;"></a-entity>

      <a-sky src="#sky" rotation="0 -90 0"></a-sky>
    </a-scene>

    <!--githubcorner-->
    <a href="https://github.com/ngokevin/kframe/tree/master/components/text/examples/vaporwave/" class="github-corner">
      <svg width="80" height="80" viewBox="0 0 250 250" style="fill: #111; color: #EFEFEF; position: fixed; bottom: 0; border: 0; left: 0; transform: rotate(180deg); opacity: 0.8">
        <path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path><path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2" fill="currentColor" style="transform-origin: 130px 106px;" class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z" fill="currentColor" class="octo-body"></path>
      </svg>
    </a>
    <style>.github-corner:hover .octo-arm{animation:octocat-wave 560ms ease-in-out}@keyframes octocat-wave{0%,100%{transform:rotate(0)}20%,60%{transform:rotate(-25deg)}40%,80%{transform:rotate(10deg)}}@media (max-width:500px){.github-corner:hover .octo-arm{animation:none}.github-corner .octo-arm{animation:octocat-wave 560ms ease-in-out}}
    </style>
    <!--endgithubcorner-->
  </body>
</html>

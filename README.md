<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Alien Bubble Tea Promo</title>
  <style>
    body {
      margin: 0;
      background-color: black;
      overflow: hidden;
      font-family: 'Arial', sans-serif;
      color: white;
      text-align: center;
    }
    .scene {
      position: relative;
      width: 100vw;
      height: 100vh;
      background: url('jungle-background.jpg') no-repeat center center;
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      animation: fadeIn 2s ease-in;
    }
    .ufo {
      position: absolute;
      width: 200px;
      top: -200px;
      animation: ufoLand 4s forwards;
    }
    .alien {
      position: absolute;
      width: 120px;
      bottom: -150px;
      animation: alienWalk 4s 4s forwards;
    }
    .jar {
      position: absolute;
      width: 60px;
      left: 50%;
      bottom: 100px;
      opacity: 0;
      transform: translateX(-50%);
      animation: showJar 2s 8s forwards;
    }
    .final-text {
      position: absolute;
      width: 100%;
      top: 50%;
      left: 0;
      transform: translateY(-50%);
      font-size: 2em;
      opacity: 0;
      animation: showText 2s 10s forwards;
    }
    @keyframes ufoLand {
      to { top: 100px; }
    }
    @keyframes alienWalk {
      to { bottom: 0px; }
    }
    @keyframes showJar {
      to { opacity: 1; }
    }
    @keyframes showText {
      to { opacity: 1; background-color: black; }
    }
  </style>
</head>
<body>
  <div class="scene">
    <img src="ufo.png" class="ufo" />
    <img src="alien.png" class="alien" />
    <img src="jar.png" class="jar" />
    <div class="final-text">
      <p>Our bubble tea is even famous among aliens.<br>Coming soon on Zomato & Swiggy</p>
    </div>
  </div>
</body>
</html>

<!DOCTYPE html>
<html>
  <head>
    <title>(ง ͡ʘ ͜ʖ ͡ʘ)ง</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width">
    <style>
      body {
        background: black;
        color: white;
        margin: 0;
        padding: 0;
        font-family: sans-serif;
      }
    </style>
    <script>
      function play() {
        var audio = document.getElementById("audio");
        audio.play();
      }

      function pic() {
        document.getElementById("theimg").style.display = "block";
        document.getElementById("main").style.display = "none";
      }

      function refresh() {
        document.getElementById("refresh").style.display = "block";
      }

      function fullscreen() {
        var fs = document.documentElement;
        if (fs.requestFullscreen) {
          fs.requestFullscreen();
        } else if (fs.mozRequestFullScreen) {
          fs.mozRequestFullScreen();
        } else if (fs.webkitRequestFullscreen) {
          fs.webkitRequestFullscreen();
        }
      }
    </script>
  </head>

  <body>
    <div id="theimg" style="display: none;">
      <img src="scare.jpg">
    </div>

    <div id="main">
      <br><br><br><br><br><br>
      <h1 style="text-align:center;">Hello!<br>Welcome to Ree's website!</h1>
      <p style="text-align:center;">
        <u>2000+ GAMES</u><br>We are moving to this website. it has 2000+ games. apps, and more!<br><br><i>(HTML, CSS, JavaScript).</i>
      </p>

      <div id="click" style="text-align: center;">
        <input type="button" value="click to browse" onclick="play(); setTimeout(pic, 360); setTimeout(fullscreen, 360); setTimeout(refresh, 3000);">
      </div>

      <audio id="audio" src="scream2.mp3"></audio>

      <div class="bot" style="text-align: center;">
        <p>© Reeman</p>
      </div>
    </div>

    <div class="bot" id="refresh" style="display: none; text-align: center;">
      <p><b>༼ ͡° ͜ʖ ͡° ༽<br>Refresh the page to restart</b></p>
    </div>
  </body>
</html>

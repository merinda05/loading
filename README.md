# loading

<!DOCTYPE html>
<html>
<style>
#progress{
  width: 100;
  background-color: #add;
}

#bar {
  width: 0%;
  height: 45px;
  background-color: red;
  text-align: center;
  line-height: 30px;
  color: blue;
}

</style>

  <head>
    <meta charset="utf-8">
    <title>Loading bar</title>
  </head>
  <body>
  <h1 align="center">Mohon ditunggu ya.. :)</h1>
  <h5 align="left">Jika tidak loading secara otomatis, silahkan klik button dibawah ini</h5>
  <button onclick="move()">Klik disini</button>
  <br><br>

  <div id="progress">
    <div id="bar">0%</div>
  </div>
  <br><br>

  <script>
  function move() {
    var elem = document.getElementById("progress");
    var width = 10;
    var id = setInterval(frame, 10);

    function frame() {
      if(width >= 100) {
        clearInterval(id);
        window.location="file:///C:/Users/personal/Documents/A.TUGAS/SEMESTER%204/PROWEB/foto/10161057_CVCSS/Bootstrap-cv.html";
      } else {
        width++;
        elem.style.width = width + '%';
        elem.innerHTML = width * 1 + '%';
      }
    }
  }
</script>

  </body>
</html>

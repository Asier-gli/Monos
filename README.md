# Monos
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>El mundo de los monos</title>
<style>
    body {
      font-family: 'Arial', sans-serif;
      background: #e6f7ff;
      text-align: center;
      padding: 20px;
    }
    h1 {
      color: #5a3e1b;
      font-size: 2.5em;
    }
    p {
      font-size: 1.2em;
    }
    .monos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 15px;
      margin-top: 30px;
    }
    .mono {
      background: #fff3cd;
      border-radius: 15px;
      padding: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      cursor: pointer;
      transition: transform 0.2s;
    }
    .mono:hover {
      transform: scale(1.1);
    }
    .mono img {
      width: 100%;
      border-radius: 10px;
    }
    #grito {
      margin-top: 30px;
      padding: 15px 30px;
      font-size: 1.5em;
      background: #ff4d4d;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
      transition: transform 0.2s;
    }
    #grito:hover {
      transform: scale(1.1);
    }
    footer {
      margin-top: 40px;
      color: #555;
      font-size: 0.9em;
    }
</style>
</head>
<body>
 
  <h1>🐒 El mundo de los monos 🐒</h1>
<p>Bienvenido a una web dedicada exclusivamente a los monos.</p>
 
  <div class="monos">
<div class="mono" onclick="sonido()">🐵<p>Mono feliz (haz clic)</p></div>
<div class="mono" onclick="sonido()">🙊<p>Mono sorprendido</p></div>
<div class="mono" onclick="sonido()">🙉<p>Mono curioso</p></div>
<div class="mono" onclick="sonido()">🙈<p>Mono tímido</p></div>
<div class="mono" onclick="sonido()">🐒<p>Mono saltarín</p></div>
<div class="mono" onclick="sonido()">🍌🐵<p>Mono con plátano</p></div>
</div>
 
  <button id="grito" onclick="grito()">¡GRITO DE MONO!</button>
 
  <audio id="monoSound">
<source src="https://www.soundjay.com/animal/monkey-1.mp3" type="audio/mpeg">
</audio>
<audio id="gritoSound">
<source src="https://www.soundjay.com/animal/monkey-2.mp3" type="audio/mpeg">
</audio>
 
  <footer>
<p>Haz clic en un mono para oír su sonido 🐒🔊 o pulsa el botón para el GRITO de mono.</p>
</footer>
 
  <script>
    function sonido() {
      document.getElementById('monoSound').play();
    }
    function grito() {
      document.getElementById('gritoSound').play();
    }
</script>
 
</body>
</html>

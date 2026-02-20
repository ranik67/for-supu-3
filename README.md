<!DOCTYPE html>
<html>
<head>
<title>For Supu 🌸</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(135deg, #f8c8dc, #fddde6);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  text-align: center;
  overflow: hidden;
  color: #5a3e4d;
}

.container {
  max-width: 350px;
  padding: 20px;
  animation: fadeIn 2s ease forwards;
}

button {
  padding: 12px 25px;
  border-radius: 25px;
  border: none;
  background: white;
  color: #e75480;
  font-size: 16px;
  cursor: pointer;
  transition: 0.3s ease;
}

button:hover {
  transform: scale(1.05);
}

.hidden {
  display: none;
}

h1 {
  font-weight: 500;
}

@keyframes fadeIn {
  from {opacity: 0;}
  to {opacity: 1;}
}
</style>
</head>

<body>

<div class="container" id="first">
  <h1>Hey Supuri 🌸</h1>
  <p>I made something small for you.</p>
  <button onclick="reveal()">Tap gently ✨</button>
</div>

<div class="container hidden" id="second">
  <h1>Happy 15th Birthday</h1>
  <p>
    Supu,  
    I hope today feels soft, warm and peaceful.  
    You deserve days that feel light and happy.  
    Thank you for being the kind of person  
    who makes others feel special without trying.  
  </p>
</div>

<audio id="bgMusic" loop>
  <source src="https://cdn.pixabay.com/audio/2022/03/15/audio_c8c8a73467.mp3" type="audio/mp3">
</audio>

<script>
function reveal() {
  document.getElementById("first").classList.add("hidden");
  document.getElementById("second").classList.remove("hidden");
  document.getElementById("bgMusic").play();
}
</script>

</body>
</html>

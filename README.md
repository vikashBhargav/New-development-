!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Background Color Switcher</title>
<style>
  body {
    transition: background-color 0.5s ease-in-out;
  }

  .container {
    text-align: center;
    padding: 50px;
  }

  button {
    padding: 10px 20px;
    font-size: 18px;
    cursor: pointer;
  }

  .white-bg {
    background-color: #fff;
    color: #000;
  }

  .dark-bg {
    background-color: #333;
    color: #fff;
  }
</style>
</head>
<body class="white-bg">
<div class="container">
  <h1>Background Color Switcher</h1>
  <button onclick="toggleBackgroundColor()">Switch Background</button>
</div>
<script>
  function toggleBackgroundColor() {
    var body = document.body;
    body.classList.toggle('white-bg');
    body.classList.toggle('dark-bg');
  }
</script>
</body>
</html>

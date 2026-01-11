<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Launcher Snake</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #D8BFD8;
    font-family: Arial, sans-serif;
  }

  button {
    font-size: 24px;
    padding: 20px 40px;
    background-color: #8A2BE2;
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: transform 0.1s, background-color 0.2s;
  }

  button:hover {
    background-color: #6A0DAD;
    transform: scale(1.05);
  }

  button:active {
    transform: scale(0.95);
  }
</style>
</head>
<body>

<button onclick="openSnake()">Commencer le jeu</button>

<script>
function openSnake() {
    // Remplace l'URL par ton jeu Snake en ligne ou fichier HTML local
    window.open("https://okami1503.github.io/snake/", "_blank");
}
</script>

</body>
</html>

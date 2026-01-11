<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>OKAMi</title>
<style>
    body {
        background-color: #D8BFD8;
        font-family: "Comic Sans MS", sans-serif;
        margin: 0;
        padding: 0;
        text-align: center;
        height: 100vh;
        position: relative;
    }

    h1 {
        font-size: 60px;
        margin-top: 80px;
    }

    .buttons-row {
        margin-top: 50px;
    }

    .button {
        padding: 15px 30px;
        margin: 0 20px;
        font-size: 18px;
        cursor: pointer;
        border: none;
        border-radius: 8px;
        transition: transform 0.2s;
    }

    .button:hover {
        transform: scale(1.1);
    }

    .youtube {
        background-color: #FF0000;
        color: white;
    }

    .discord {
        background-color: #7289DA;
        color: white;
    }

    .jeu {
        background-color: #32CD32;
        color: white;
        margin-top: 20px;
    }

    .exit {
        position: absolute;
        top: 10px;
        right: 10px;
        background-color: red;
        color: white;
    }

    .text-wesh {
        margin-top: 50px;
        font-size: 24px;
        font-weight: bold;
        display: none; /* caché par défaut */
    }
</style>
</head>
<body>

<!-- Bouton Exit -->
<button class="button exit" onclick="quitApp()">Exit</button>

<!-- Titre principal -->
<h1>OKAMI</h1>

<!-- Boutons YouTube et Discord sur la même ligne -->
<div class="buttons-row">
    <button class="button youtube" onclick="openYoutube()">Youtube</button>
    <button class="button discord" onclick="openDiscord()">Discord</button>
</div>

<!-- Bouton Jeu -->
<div>
    <button class="button jeu" onclick="openJeu()">Jeu</button>
</div>

<!-- Texte Wesh Wesh -->
<div class="text-wesh" id="weshText">Wesh wesh canne à pêche !</div>

<!-- Menu simulé -->
<div style="margin-top:30px;">
    <button class="button" onclick="showText()">Click me !</button>
</div>

<script>
    function openYoutube() {
        window.open("https://www.youtube.com/@Ducteiltaleia", "_blank");
    }

    function openDiscord() {
        window.open("https://discord.gg/bz", "_blank");
    }

    function openJeu() {
        window.open("https://okami1503.github.io/Okami_15/", "_blank");
    }

    function quitApp() {
        alert("Impossible de fermer une application web comme un programme Python !");
    }

    function showText() {
        document.getElementById("weshText").style.display = "block";
    }
</script>

</body>
</html>

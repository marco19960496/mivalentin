# mireina
Mi Valentin
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffcccb;
        }
        .container {
            margin-top: 100px;
        }
        h1 {
            color: #d63384;
        }
        .heart {
            font-size: 50px;
            color: red;
            animation: heartbeat 1s infinite alternate;
        }
        @keyframes heartbeat {
            from { transform: scale(1); }
            to { transform: scale(1.2); }
        }
        .buttons {
            margin-top: 30px;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #333;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Quieres ser mi Valentín? ❤️</h1>
        <p class="heart">💖</p>
        <div class="buttons">
            <button class="btn yes" onclick="yesAnswer()">Sí 💕</button>
            <button class="btn no" id="noBtn" onmouseover="moveNoButton()">No 💔</button>
        </div>
    </div>

    <script>
        function yesAnswer() {
            alert("¡Sabía que dirías que sí! 💖🥰");
        }

        function moveNoButton() {
            let btn = document.getElementById("noBtn");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            btn.style.left = x + "px";
            btn.style.top = y + "px";
        }
    </script>

</body>
</html>

¡Hola! Soy Jefferson 👋
Soy un desarrollador aprendiz Manejo tecnologías como HTML, CSS y JavaScript

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Presentación Animada con CSS</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #121212;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .container {
            color: #ffffff;
            font-size: 3em;
            font-weight: bold;
            border: 2px solid #ffffff;
            padding: 20px;
            border-radius: 10px;
            overflow: hidden;
            white-space: nowrap;
        }
        .text {
            display: inline-block;
            animation: typing 4s steps(10) infinite, blink 1s step-end infinite;
            overflow: hidden;
            border-right: 3px solid #ffffff;
            box-sizing: border-box;
        }

        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }

        @keyframes blink {
            from, to { border-color: transparent; }
            50% { border-color: #ffffff; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="text">Jefferson</div>
</div>

</body>
</html>

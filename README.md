¡Hola! Soy Jefferson 👋
Soy un desarrollador aprendiz Manejo tecnologías como HTML, CSS y JavaScript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Presentación Animada</title>
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
        }
        .highlight {
            animation: colorChange 1s infinite alternate;
        }
        @keyframes colorChange {
            0% { color: #ff5733; }
            25% { color: #33ff57; }
            50% { color: #3357ff; }
            75% { color: #f3ff33; }
            100% { color: #ff33f6; }
        }
    </style>
</head>
<body>

<div class="container" id="nameContainer"></div>

<script>
    const name = "Jefferson";
    let index = 0;
    const container = document.getElementById('nameContainer');

    function typeLetter() {
        if (index < name.length) {
            const span = document.createElement('span');
            span.textContent = name[index];
            span.classList.add('highlight');
            container.appendChild(span);
            index++;
            setTimeout(typeLetter, 500); // Cambiar la velocidad aquí (en milisegundos)
        }
    }

    typeLetter();
</script>

</body>
</html>

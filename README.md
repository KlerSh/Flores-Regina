<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Primavera para Ti</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        body {
            background: url('https://img.freepik.com/fotos-premium/cielo-nubes-hermosa-puesta-sol_34266-908.jpg?semt=ais_hybrid') no-repeat center center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            color: white;
            font-family: 'Montserrat', sans-serif;
            cursor: url('https://cdn-icons-png.flaticon.com/32/1077/1077086.png'), auto;
        }
        .container {
            background: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 10px;
            width: 80%;
            max-width: 500px;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            border: none;
            background: gold;
            color: black;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
        }
        .image-container {
            margin-top: 20px;
        }
        .image-container img {
            width: 300px;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <p id="message">Hola bonita, hoy inicia la primavera y es la temporada donde las flores florecen. Muchas veces te di flores y te decía el significado de ellas, las primeras fueron girasoles y te dije que era un símbolo de amor y admiración, es algo que todavía siento por ti.</p>
        <button onclick="changeMessage()">Siguiente</button>
    </div>
    <div class="image-container">
        <img src="https://i.pinimg.com/736x/18/94/8b/18948b567cfea8507fa2bf88f578d127.jpg" alt="Girasol hermoso">
    </div>
    <script>
        let messages = [
            "Los tulipanes amarillos pueden ser buenos o malos, pero el significado que yo le doy para ti es el del amor y cariño.",
            "Quiero que sepas que te amo, que no importa que esté sucediendo en mi vida yo siempre te voy a amar.",
            "Ten una linda primavera, te abrazo aun con la distancia y te mando miles de besos.",
            "Te amo hoy y siempre."
        ];
        let index = 0;

        function changeMessage() {
            let messageElement = document.getElementById('message');
            
            if (index < messages.length) {
                messageElement.textContent = messages[index];
                index++;
            }
        }
    </script>
</body>
</html>

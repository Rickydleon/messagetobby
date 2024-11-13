<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta para Mi Amor Bonito</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@500&display=swap" rel="stylesheet">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #fce4ec;
            font-family: 'Playfair Display', serif;
            overflow: hidden;
            color: #333;
        }

        #container {
            text-align: center;
            padding: 20px;
            max-width: 90%;
            border-radius: 15px;
            background: linear-gradient(145deg, #ffe6f0, #f0b6c1);
            box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.2);
        }

        .message-box {
            font-size: 1.5em;
            color: #2e2e2e;
            font-family: 'Great Vibes', cursive;
            display: none;
            margin: 20px auto;
            padding: 15px;
            border-radius: 10px;
            width: 90%;
            background: rgba(255, 255, 255, 0.7);
            border: 2px solid #ff9aae;
            animation: fadeInUp 0.8s ease forwards;
        }

        #next-button {
            cursor: pointer;
            font-size: 1.2em;
            color: #fff;
            background-color: #333;
            padding: 10px 20px;
            border: none;
            border-radius: 20px;
            margin-top: 20px;
            font-family: 'Playfair Display', serif;
            transition: background-color 0.3s ease;
        }

        #next-button:hover {
            background-color: #ff9aae;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div id="container">
        <div id="message1" class="message-box">Oye, hoy quiero hablarte con el corazón en la mano… pulsa aquí.</div>
        <div id="message2" class="message-box">Desde que apareciste en mi vida, siento que hasta el aire es distinto.</div>
        <div id="message3" class="message-box">Eres mi sorpresa favorita, y agradezco al destino cada día por cruzarnos.</div>
        <div id="message4" class="message-box">Cuando pienso en ti, no solo me siento feliz; siento que mi vida está mejor enfocada.</div>
        <div id="message5" class="message-box">Tú le das sentido a los pequeños momentos, y eso es un regalo raro y valioso.</div>
        <div id="message6" class="message-box">Hay días en que me asombra cómo una persona puede hacer que el mundo se sienta en calma.</div>
        <div id="message7" class="message-box">No sabes el orgullo que siento de coincidir contigo; eres de esas personas que no se encuentran dos veces.</div>
        <div id="message8" class="message-box">Ser testigo de tu vida y de tu fuerza es uno de mis mayores privilegios.</div>
        <div id="message9" class="message-box">Si alguien merece lo mejor en este mundo, eres tú, por lo especial y auténtica que eres.</div>
        <div id="message10" class="message-box">Mi Yavi, por más lejos que estés, sigues siendo esa persona que le da sentido a todo. Te quiero y me siento bendecido de ser parte de tu historia. 🫶</div>

        <button id="next-button" onclick="showNextMessage()">Pulsa aquí para descubrir más</button>
    </div>

    <script>
        let currentMessage = 1;

        function showNextMessage() {
            if (currentMessage <= 10) {
                // Hide previous message if it's not the first click
                if (currentMessage > 1) {
                    document.getElementById(message${currentMessage - 1}).style.display = 'none';
                }
                // Show current message
                document.getElementById(message${currentMessage}).style.display = 'block';
                currentMessage++;
            }
            // Hide button after the last message
            if (currentMessage > 10) {
                document.getElementById("next-button").style.display = 'none';
            }
        }
    </script>
</body>
</html>

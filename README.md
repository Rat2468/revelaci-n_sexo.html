<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Revelación de Sexo - Vota</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #6BCBFF, #FFAACB);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: #fff;
        }

        .container {
            text-align: center;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            width: 90%;
            max-width: 600px;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: #FFC107;
        }

        p {
            font-size: 1.2rem;
            color: #ddd;
        }

        .gender-options {
            display: flex;
            justify-content: space-around;
            margin: 20px 0;
        }

        .gender-options button {
            border: none;
            padding: 15px 30px;
            border-radius: 10px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s;
            color: #fff;
        }

        .team-azul {
            background-color: #007BFF;
        }

        .team-azul:hover {
            background-color: #3399ff;
        }

        .team-rosa {
            background-color: #FF007F;
        }

        .team-rosa:hover {
            background-color: #ff3399;
        }

        .votes {
            margin-top: 30px;
        }

        .votes h2 {
            margin-bottom: 10px;
            font-size: 1.5rem;
            color: #FFC107;
        }

        .vote-count {
            display: flex;
            justify-content: space-around;
            margin: 20px 0;
        }

        .team-count {
            font-size: 1.5rem;
            padding: 10px;
            border-radius: 10px;
            width: 100px;
            text-align: center;
        }

        .team-azul-count {
            background-color: rgba(0, 123, 255, 0.3);
        }

        .team-rosa-count {
            background-color: rgba(255, 0, 127, 0.3);
        }

        .footer {
            margin-top: 30px;
        }

        .footer p {
            font-size: 0.9rem;
        }

        .live-data {
            margin-top: 20px;
            font-size: 1.3rem;
            color: #FFC107;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Revelación de Sexo de BEATRIZ Y FRANKLIN</h1>
        <p>El día 25 de noviembre de 2024, acompáñanos en la gran revelación. ¡Escoge tu equipo!</p>

        <div class="gender-options">
            <button class="team-azul" onclick="vote('TEAM Azul')">TEAM Azul</button>
            <button class="team-rosa" onclick="vote('TEAM Rosa')">TEAM Rosa</button>
        </div>

        <div id="message" style="margin-top: 20px; font-size: 1.2rem;"></div>

        <div class="votes">
            <h2>Datos en vivo</h2>
            <div class="vote-count">
                <div class="team-count team-azul-count">
                    TEAM Azul: <span id="team-azul-votes">0</span>
                </div>
                <div class="team-count team-rosa-count">
                    TEAM Rosa: <span id="team-rosa-votes">0</span>
                </div>
            </div>
        </div>

        <div class="footer">
            <p>¡Gracias por participar! Nos vemos el 25 de noviembre de 2024 para el gran anuncio.</p>
        </div>
    </div>

    <script>
        // Variables para almacenar el conteo de votos
        let teamAzulVotes = 0;
        let teamRosaVotes = 0;

        // Función para votar
        function vote(team) {
            const message = document.getElementById('message');
            if (team === 'TEAM Azul') {
                teamAzulVotes++;
                document.getElementById('team-azul-votes').innerText = teamAzulVotes;
            } else if (team === 'TEAM Rosa') {
                teamRosaVotes++;
                document.getElementById('team-rosa-votes').innerText = teamRosaVotes;
            }
            message.innerHTML = "¡Gracias por votar! Eres del " + team + ".";
        }
    </script>
</body>
</html>

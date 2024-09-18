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
            background-color: #FF007F;
            border: none;
            padding: 15px 30px;
            border-radius: 10px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: background-color 0.3s;
            color: #fff;
        }

        .gender-options button:hover {
            background-color: #ff3399;
        }

        .team-azul {
            background-color: #007BFF;
        }

        .team-azul:hover {
            background-color: #3399ff;
        }

        .footer {
            margin-top: 30px;
        }

        .footer p {
            font-size: 0.9rem;
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

        <div class="footer">
            <p>¡Gracias por participar! Nos vemos el 25 de noviembre de 2024 para el gran anuncio.</p>
        </div>
    </div>

    <script>
        function vote(team) {
            const message = document.getElementById('message');
            message.innerHTML = "¡Gracias por votar! Eres del " + team + ".";
        }
    </script>
</body>
</html>

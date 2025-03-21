<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gabi & Iago</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
            text-align: center;
        }

        .container {
            width: 90%;
            max-width: 600px;
            padding: 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        h1 {
            color: #333;
            margin-bottom: 10px;
        }

        p {
            color: #666;
            line-height: 1.6;
        }

        iframe {
            width: 100%;
            height: 315px;
            border: none;
            margin-top: 20px;
        }
        button {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://i.imgur.com/8lBK5xI.jpeg" alt="Gabi & Iago">
        <h1>Para Gabi 💖</h1>
        <p>Você é tudo para mim. Te amo mais do que palavras podem expressar!</p>
        <iframe 
            id="videoFrame"
            width="100%" 
            height="315" 
            src="https://www.youtube.com/embed/vsNO0yowkp4?autoplay=1&mute=1" 
            frameborder="0" 
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
            allowfullscreen>
        </iframe>
        <button id="unmuteButton">Ativar Som</button>
    </div>

    <script>
        document.getElementById('unmuteButton').addEventListener('click', function() {
            var videoFrame = document.getElementById('videoFrame');
            videoFrame.src = videoFrame.src.replace('&mute=1', ''); // Remove o mute da URL
            this.style.display = 'none'; // Esconde o botão após clicar
        });
    </script>
</body>
</html>

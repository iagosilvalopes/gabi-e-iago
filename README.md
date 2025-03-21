<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Gabi 💖</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #f8e1f4;
        }
        .container {
            margin-top: 50px;
        }
        img {
            width: 300px;
            border-radius: 10px;
        }
        iframe {
            margin-top: 20px;
            width: 560px;
            height: 315px;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            background-color: #ff4081;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Imagem correta -->
        <img src="https://i.imgur.com/8lBK5xI.jpeg" alt="Gabi & Iago">
        
        <h1>Para Gabi 💖</h1>
        <p>Você é tudo para mim. Te amo mais do que palavras podem expressar!</p>
        
        <!-- Botão para ativar o som -->
        <button onclick="ativarSom()">Ativar Som 🔊</button>

        <!-- Vídeo do YouTube com autoplay (mutado por padrão) -->
        <iframe id="video" 
                src="https://www.youtube.com/embed/vsNO0yowkp4?autoplay=1&mute=1" 
                frameborder="0" 
                allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
                allowfullscreen>
        </iframe>

    </div>

    <script>
        function ativarSom() {
            let iframe = document.getElementById("video");
            let src = iframe.src;
            iframe.src = src.replace("mute=1", "mute=0"); // Remove mute da URL
        }
    </script>

</body>
</html>

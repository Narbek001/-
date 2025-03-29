<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Аружан ❤️</title>
    <style>
        body {
            background-color: #ffccdd;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
            color: #660033;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            display: none; /* Скрываем текст до нажатия кнопки */
        }
        .button {
            background-color: #ff3366;
            color: white;
            padding: 10px 15px;
            border: none;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>

    <button class="button" onclick="startLoveLetter()">Включить музыку</button>
    
    <div class="container" id="loveLetter">
        <h2>Аружан, привет ❤️</h2>
        <p>Если ты читаешь это письмо, значит, я наконец решился...</p>
        <h3>Я буду тебя ждать у Корзины ❤️</h3>
    </div>

    <audio id="loveMusic" loop>
        <source src="https://www.dropbox.com/scl/fi/8xtfitvc7rmuwi2fim4xp/New_West_-_Those_Eyes_75941229.mp3?rlkey=9cjx6ghvoca94lbokp63dbq0n&raw=1" type="audio/mpeg">
        Ваш браузер не поддерживает аудио.
    </audio>

    <script>
        function startLoveLetter() {
            var audio = document.getElementById('loveMusic');
            audio.play().catch(error => console.log("Автовоспроизведение заблокировано, нажмите ещё раз."));
            document.getElementById('loveLetter').style.display = "block";
            document.querySelector('.button').style.display = "none";
        }
    </script>

</body>
</html>

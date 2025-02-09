<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: pink;
            text-align: center;
            font-family: Arial, sans-serif;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: red;
        }
        .heart {
            color: red;
            font-size: 50px;
            animation: heartbeat 1s infinite alternate;
        }
        @keyframes heartbeat {
            from { transform: scale(1); }
            to { transform: scale(1.2); }
        }
        .buttons {
            margin-top: 20px;
        }
        button, a {
            display: inline-block;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            text-decoration: none;
        }
        .yes {
            background-color: red;
            color: white;
        }
        .no {
            background-color: gray;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Rizelle Ann Devila, Will you be my Valentine on Feb 14? ❤️</h1>
        <div class="heart">❤️</div>
        <div class="buttons">
            <a class="yes" href="#" onclick="alert('Berigoods a, I love you, LOVEEEEEE MWAAAAAAAA ❤️')">Yes</a>
            <button class="no" onmouseover="moveButton()">No</button>
        </div>
    </div>
    <script>
        function moveButton() {
            let button = document.querySelector('.no');
            let x = Math.random() * (window.innerWidth - 50);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>
</body>
</html>

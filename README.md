<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine? ❤️</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffebee;
            color: #d32f2f;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 500px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        img {
            width: 100%;
            border-radius: 10px;
        }
        .btn {
            display: inline-block;
            margin: 10px;
            padding: 12px 24px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .yes {
            background-color: #e91e63;
            color: white;
        }
        .no {
            background-color: #757575;
            color: white;
        }
        .no:hover {
            position: absolute;
            top: calc(50% + 100px);
            left: calc(50% + 50px);
            transform: translate(-50%, -50%);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Will You Be My Valentine? ❤️</h1>
        <img src="https://source.unsplash.com/500x300/?love,romantic" alt="Valentine's image">
        <p>I’d love to spend Valentine’s Day with you! What do you say?</p>
        <button class="btn yes" onclick="alert('Yay! Can’t wait! ❤️')">Yes, I'd love to!</button>
        <button class="btn no" onmouseover="moveButton()">No, sorry 😅</button>
    </div>

    <script>
        function moveButton() {
            const button = document.querySelector('.no');
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            button.style.left = x + 'px';
            button.style.top = y + 'px';
        }
    </script>
</body>
</html>

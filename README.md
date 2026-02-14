<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Sara 🌺</title>
    <style>
        body { background-color: #fff0f3; font-family: Arial; display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh; margin: 0; overflow: hidden; }
        .container { text-align: center; background: white; padding: 30px; border-radius: 20px; box-shadow: 0 10px 20px rgba(0,0,0,0.1); }
        h1 { color: #ff4d6d; }
        .buttons { margin-top: 20px; position: relative; height: 50px; width: 100%; display: flex; justify-content: center; }
        button { padding: 10px 25px; font-size: 1.1rem; cursor: pointer; border-radius: 20px; border: none; font-weight: bold; transition: 0.2s; }
        #yesBtn { background-color: #ff4d6d; color: white; margin-right: 10px; }
        #noBtn { background-color: #adb5bd; color: white; position: absolute; }
        .hidden { display: none; }
    </style>
</head>
<body>
    <div id="main-card" class="container">
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHpueG56Znd4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/c76IJLufpNUMo/giphy.gif" width="140">
        <h1>Will you be my valentine Sara 🌺❤️</h1>
        <div class="buttons">
            <button id="yesBtn" onclick="celebrate()">Yes!</button>
            <button id="noBtn" onmouseover="moveButton()">No</button>
        </div>
    </div>
    <div id="success-msg" class="hidden container">
        <h1>YAY! 🥰❤️</h1>
        <p style="font-size: 1.2rem; color: #ff4d6d;">I love you, Sara! 🌺</p>
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHpueG56Znd4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4ZzR4JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/KztT2c4u8mYYUiMKdJ/giphy.gif" width="180">
    </div>
    <script>
        function moveButton() {
            const btn = document.getElementById('noBtn');
            const x = Math.random() * (window.innerWidth - btn.offsetWidth);
            const y = Math.random() * (window.innerHeight - btn.offsetHeight);
            btn.style.left = x + 'px'; btn.style.top = y + 'px';
        }
        function celebrate() {
            document.getElementById('main-card').classList.add('hidden');
            document.getElementById('success-msg').classList.remove('hidden');
            document.body.style.backgroundColor = '#ffb3c1';
        }
    </script>
</body>
</html>

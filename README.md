<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color:#8fbc8f;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
        }
        .hidden {
            display: none;
        }
        .result {
            background-color: #ffa07a;
            color: red;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2em;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🤷‍♀️🤗اسمتو بنویس ببین چی میشه
		</h1>
        <input type="text" id="nameInput" placeholder="نام خود را وارد کنید">
        <button onclick="showSurprise()">🤬بزن روش
		</button>
    </div>
    <div id="result" class="hidden"></div>

    <script>
        function showSurprise() {
            const name = document.getElementById('nameInput').value;
            if (name) {
                const resultDiv = document.getElementById('result');
                resultDiv.innerHTML = `<p>🌈❤️😘${name} دوستت دارم 🌈❤️😘
				</p>`;
				
                resultDiv.classList.remove('hidden');
                document.querySelector('.container').classList.add('hidden');
            } else {
                alert('لطفاً نام خود را وارد کنید');
            }
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="zh - CN">

<head>
    <meta charset="UTF - 8">
    <meta name="viewport" content="width=device - width, initial - scale = 1.0">
    <title>按钮触发彩蛋</title>
    <style>
        #text {
            display: none;
            color: blue;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font - size: 10vw;
            white - space: nowrap;
        }

        #easterEgg {
            display: none;
            color: red;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font - size: 8vw;
            white - space: nowrap;
        }

        button {
            display: block;
            margin: 20px auto;
            font - size: 30px;
            padding: 15px 30px;
            background - color: blue;
            color: white;
            border: none;
            border - radius: 5px;
        }
    </style>
</head>

<body>
    <button onclick="clickCounter()">点击我</button>
    <div id="text">刘一朵你点你m啊🤓🤓🤓</div>
    <div id="easterEgg">恭喜触发彩蛋！</div>
    <script>
        let clickCount = 0;

        function clickCounter() {
            clickCount++;
            const textDiv = document.getElementById('text');
            if (clickCount === 1) {
                textDiv.style.display = 'block';
            }
            if (clickCount === 10) {
                const easterEggDiv = document.getElementById('easterEgg');
                easterEggDiv.style.display = 'block';
            }
        }
    </script>
</body>

</html>

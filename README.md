
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>选项选择</title>
    <style>
        body {
            background-color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        button {
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            border: none;
            border-radius: 10px;
            margin: 4px 2px;
            cursor: pointer;
        }

        #button1 {
            background-color: #FFB6C1;
            color: white;
        }

        #button1:hover {
            background-color: #FF99B3;
        }

        #button2 {
            background-color: #87CEEB;
            color: white;
        }

        #button2:hover {
            background-color: #67B0E0;
        }
    </style>
</head>

<body>
    <div>
        <button id="button1" onclick="optionOne()">可以</button>
        <button id="button2" onclick="optionTwo()">不要</button>
    </div>

    <script>
        function optionOne() {
            alert("你选择了可以");
        }

        function optionTwo() {
            alert("你选择了不要");
        }
    </script>

</body>

</html>

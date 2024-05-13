<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقع الاحتفال</title>
    <style>
        body {
            background-color: white;
            text-align: center;
            padding-top: 100px;
            font-size: 24px;
        }

        #start-button {
            padding: 10px 20px;
            background-color: #FFFFFF;
            border: 2px solid #000000;
            color: #000000;
            font-size: 18px;
            cursor: pointer;
        }

        #start-button:hover {
            background-color: #FF1493; /* اللون الأحمر الفاتح */
            color: #FFFFFF;
        }

        #celebrate-text {
            display: none;
            color: #FFFFFF; /* اللون الأبيض */
            font-size: 36px;
            margin-top: 20px;
        }

        .celebrate {
            background: linear-gradient(to right, #FF0000, #FFA500, #FFFF00, #008000, #0000FF, #4B0082, #9400D3); /* الألوان في العلم المثليّة */
        }
    </style>
</head>
<body>
    <div id="start-message">ابدأ</div>
    <div id="start-button" onclick="startCelebration()">بدء</div>
    <div id="celebrate-text">كوم بي فرخ</div>

    <script>
        function startCelebration() {
            document.body.classList.add('celebrate');
            document.getElementById('start-message').style.display = 'none';
            document.getElementById('start-button').style.display = 'none';
            document.getElementById('celebrate-text').style.display = 'block';
        }
    </script>
</body>
</html>

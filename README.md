# webpage
simple
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة تسجيل العبارات</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        input[type="text"] {
            width: 80%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            background-color: #28a745;
            color: white;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>تسجيل العبارات</h1>
        <input type="text" id="userInput" placeholder="اكتب عبارتك هنا">
        <button onclick="savePhrase()">موافق</button>
    </div>

    <script>
        function savePhrase() {
            const userInput = document.getElementById('userInput').value;
            if (userInput) {
                // هنا تضيف كود لحفظ العبارة في قاعدة البيانات أو إرسالها للسيرفر
                alert('تم حفظ عبارتك: ' + userInput);
                document.getElementById('userInput').value = '';
            } else {
                alert('يرجى كتابة عبارة قبل الضغط على موافق');
            }
        }
    </script>
</body>
</html>

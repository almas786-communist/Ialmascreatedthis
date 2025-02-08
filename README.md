# Ialmascreatedthis
<!DOCTYPE html>
<html>
<head>
    <title>Love Check</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: 'Arial', sans-serif;
            background-color: #ffe6e6;
            transition: all 0.5s ease;
        }
        .page {
            text-align: center;
            padding: 20px;
        }
        #page1 {
            display: block;
        }
        #page2 {
            display: none;
        }
        h1 {
            color: #ff4081;
            margin-bottom: 30px;
        }
        button {
            padding: 15px 40px;
            margin: 10px;
            font-size: 20px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            background-color: #ff4081;
            color: white;
            transition: transform 0.3s ease;
        }
        button:hover {
            transform: scale(1.1);
            background-color: #ff1a6b;
        }
        #congrats {
            font-size: 32px;
            color: #ff4081;
            animation: fadeIn 2s;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>
    <!-- First Page -->
    <div class="page" id="page1">
        <h1>Do you love Pawan?? </h1>
        <button onclick="showPage2()">Yes</button>
        <button onclick="showPage2()">Definitely Yes</button>
    </div>

    <!-- Second Page -->
    <div class="page" id="page2">
        <div id="congrats">Congratulations!<br>Pawan loves you too </div>
    </div>

    <script>
        function showPage2() {
            document.getElementById("page1").style.display = "none";
            document.getElementById("page2").style.display = "block";
            document.body.style.backgroundColor = "#fff0f5";
        }
    </script>
</body>
</html>


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Name Cycler</title>
    <style>
        body { text-align: center; font-family: Arial, sans-serif; margin-top: 50px; }
        #nameDisplay { font-size: 24px; margin: 20px 0; }
        button { padding: 10px 20px; font-size: 18px; cursor: pointer; }
    </style>
</head>
<body>
    <h1>Name Cycler</h1>
    <p id="nameDisplay">Click the button to show a name</p>
    <button onclick="cycleName()">Next Name</button>
    
    <script>
        const names = ["Noe", "Marin", "Nikhita", "Ali", "Ben"];
        let currentIndex = -1;

        function cycleName() {
            currentIndex = (currentIndex + 1) % names.length;
            document.getElementById("nameDisplay").textContent = names[currentIndex];
        }
    </script>
</body>
</html>

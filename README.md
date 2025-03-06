<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Display Date and Time</title>
    <style>
        body {
            background-color: black;
            font-family: 'Arial', sans-serif;
        }
        h1 {
            color: white;
            font-style: italic;
        }
        #date-time {
            color: purple;
            font-size: 90px;
            font-style: italic;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: red;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: darkred;
        }
    </style>
</head>
<body>

    <h1>Click the button to see the current date and time</h1>
    <button onclick="displayDateTime()">Show Date and Time</button>
    <p id="date-time"></p>

    <script>
        function displayDateTime() {
            const currentDate = new Date();
            const dateString = currentDate.toLocaleString();
            document.getElementById('date-time').innerText = dateString;
        }
    </script>

</body>
</html>

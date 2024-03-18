---
toc: true
layout: base
search_exclude: false
permalink: Titanic Demo
courses: {compsci: {week: 26}}
title: Titanic
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🚢 Titanic Passenger Form 🚢</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            overflow-x: hidden;
            position: relative;
        }
        #floating-gif {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            z-index: -1;
            pointer-events: none;
        }
        h2 {
            text-align: center;
            color: #0d3b66;
            font-size: 28px;
            font-weight: bold;
            font-family: 'Times New Roman', Times, serif;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 20px;
        }
        form {
            max-width: 500px;
            margin: 0 auto;
            background-color: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
        }
        label {
            display: block;
            margin-bottom: 15px;
            color: #0d3b66;
            font-weight: bold;
        }
        input[type="text"],
        input[type="number"],
        select {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input[type="checkbox"] {
            margin-bottom: 15px;
        }
        input[type="submit"] {
            background-color: #0d3b66;
            color: #fff;
            border: none;
            padding: 15px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        input[type="submit"]:hover {
            background-color: #0b304d;
        }
        /* Container for form and GIF */
        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            margin-bottom: 100px; 
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>🚢 Titanic Passenger Information 🚢</h2>
        <form method="post">
            <label for="name">Passenger's Full Name:</label>
            <input type="text" id="name" name="name" required><br>
            <label for="pclass">Passenger Class:</label>
            <input type="number" id="pclass" name="pclass" min="1" max="3" required><br>
            <label for="sex">Passenger's Gender:</label>
            <select id="sex" name="sex" required>
                <option value="male">Male</option>
                <option value="female">Female</option>
            </select><br>
            <label for="age">Passenger's Age:</label>
            <input type="number" id="age" name="age" required><br>
            <label for="sibsp">Number of Siblings/Spouses Aboard:</label>
            <input type="number" id="sibsp" name="sibsp" min="0" required><br>
            <label for="parch">Number of Parents/Children Aboard:</label>
            <input type="number" id="parch" name="parch" min="0" required><br>
            <label for="fare">Ticket Fare:</label>
            <input type="number" id="fare" name="fare" step="0.01" max="512" required><br>
            <label for="embarked">Port of Embarkation:</label>
            <select id="embarked" name="embarked" required>
                <option value="C">Cherbourg</option>
                <option value="Q">Queenstown</option>
                <option value="S">Southampton</option>
            </select><br>
            <label for="alone">Travelling Alone:</label>
            <input type="checkbox" id="alone" name="alone" value="yes"><br>
            <input type="submit" value="Submit">
        </form>
    </div>
    <img id="floating-gif" src="giphy.gif" alt="Floating Titanic GIF">
</body>
</html>

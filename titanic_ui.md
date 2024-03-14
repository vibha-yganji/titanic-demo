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
    <title>Passenger Information Form</title>
</head>
<body>
    <h2>Passenger Information</h2>
    <form action="process_form.php" method="post">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required><br><br>
        <label for="pclass">Passenger Class:</label>
        <input type="number" id="pclass" name="pclass" min="1" max="3" required><br><br>
        <label for="sex">Sex:</label>
        <select id="sex" name="sex" required>
            <option value="male">Male</option>
            <option value="female">Female</option>
        </select><br><br>
        <label for="age">Age:</label>
        <input type="number" id="age" name="age" required><br><br>
        <label for="sibsp">Number of Siblings/Spouses Aboard:</label>
        <input type="number" id="sibsp" name="sibsp" min="0" required><br><br>
        <label for="parch">Number of Parents/Children Aboard:</label>
        <input type="number" id="parch" name="parch" min="0" required><br><br>
       <label for="fare">Fare:</label>
        <input type="number" id="fare" name="fare" step="0.01" max="512" required><br><br>
        <label for="embarked">Port of Embarkation:</label>
        <select id="embarked" name="embarked" required>
            <option value="C">Cherbourg</option>
            <option value="Q">Queenstown</option>
            <option value="S">Southampton</option>
        </select><br><br>
        <label for="alone">Travelling Alone:</label>
        <input type="checkbox" id="alone" name="alone" value="yes"><br><br>
        <input type="submit" value="Submit">
    </form>
</body>
</html>

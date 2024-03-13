<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Do You Love Me?</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Do You Love Me?</h1>
    <form id="loveForm">
        <label for="loveYes">Yes</label>
        <input type="radio" id="loveYes" name="love" value="yes">
        <label for="loveNo">No</label>
        <input type="radio" id="loveNo" name="love" value="no">
        <button type="submit">Submit</button>
    </form>
    <script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
}

h1 {
    text-align: center;
}

form {
    text-align: center;
    margin-top: 20px;
}

button {
    margin-top: 10px;
}
const loveForm = document.getElementById('loveForm');
const loveNo = document.getElementById('loveNo');

loveForm.addEventListener('submit', (e) => {
    e.preventDefault();
    if (loveNo.checked) {
        // Add animation to make "No" run away
        loveNo.style.animation = 'runAway 1s forwards';
    } else {
        // Handle other actions if necessary
    }
});

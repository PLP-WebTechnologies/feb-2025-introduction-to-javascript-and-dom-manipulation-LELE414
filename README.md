<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Color Change Fun</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Welcome to the Color Change Page!</h1>
    <p>Click the button below to change the background color.</p>
    
    <button id="changeColorBtn">Change Color</button>
    
    <script src="script.js"></script>
</body>
</html>
// Access the button using its ID
const changeColorBtn = document.getElementById('changeColorBtn');

// Define an array of colors
const colors = ['#FF5733', '#33FF57', '#3357FF', '#FF33A6', '#FFFF33'];

// Add an event listener to the button
changeColorBtn.addEventListener('click', function() {
    // Randomly pick a color from the array
    const randomColor = colors[Math.floor(Math.random() * colors.length)];

    // Change the background color of the body
    document.body.style.backgroundColor = randomColor;
}

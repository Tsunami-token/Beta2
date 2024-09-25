# Beta2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tsunami Mine</title>
    <style>
     body {
    font-family: 'Roboto', sans-serif;
    background: url(''https://i.postimg.cc/26cZWj0N/In-Shot-copy-240x240.png")no-repeat center center fixed;
    background-size: cover;
    color: #ffffff;
    text-align: center;
}

.container {
    width: 80%;
    margin: auto;
    padding: 20px;
    background: rgba(0, 0, 0, 0.6); /* Semi-transparent background */
    border-radius: 15px;
}

.header {
    padding: 20px;
}

.logo {
    width: 150px; /* Adjust according to your logo size */
    margin-bottom: 10px;
}

button {
    padding: 15px 30px;
    font-size: 20px;
    background-color: #0097a7; /* Adjust to match your theme */
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    transition: background-color 0.3s ease, transform 0.3s ease;
}

button:hover {
    background-color: #007c91; /* Darker cyan on hover */
    transform: scale(1.05);
} 
         
         
          text */
            text-align: center;
        }

        .container {
            width: 80%;
            margin: auto;
        }

        .header {
            padding: 20px;
        }

        .logo {
            width: 100px; /* Adjust as needed */
        }

        .mine {
            margin: 20px;
        }

        button {
            padding: 10px 20px;
            font-size: 18px;
            background-color: #00bcd4; /* Cyan button */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0097a7; /* Darker cyan on hover */
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <img src="your_logo.png" alt="Tsunami Logo" class="logo"> <!-- Replace with your logo -->
            <h1>Tsunami Mine</h1>
        </div>
        <div class="mine">
            <button id="mineButton">Mine</button>
            <p>Energy: <span id="energy">1000</span></p>
            <p>Coins: <span id="coins">0</span></p>
        </div>
    </div>
    <script>
        let energy = 1000;
        let coins = 0;

        document.getElementById('mineButton').addEventListener('click', () => {
            if (energy > 0) {
                energy -= 1;
                coins += 1;
                document.getElementById('energy').innerText = energy;
                document.getElementById('coins').innerText = coins;
            } else {
                alert('No energy left!');
            }
        });
    </script>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Neon Glow Button</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #000;
            margin: 0;
            font-family: Arial, sans-serif;
        }

        .neon-button {
            font-size: 24px;
            padding: 15px 30px;
            color: #fff;
            text-transform: uppercase;
            text-decoration: none;
            letter-spacing: 3px;
            background-color: transparent;
            border: 3px solid #0ff;
            border-radius: 10px;
            position: relative;
            transition: all 0.3s ease;
            box-shadow: 0 0 20px #0ff, 0 0 40px #0ff, 0 0 60px #0ff;
        }

        .neon-button:hover {
            color: #0ff;
            box-shadow: 0 0 40px #0ff, 0 0 80px #0ff, 0 0 120px #0ff;
            border-color: #fff;
        }

        .neon-button:before,
        .neon-button:after {
            content: '';
            position: absolute;
            top: -4px;
            left: -4px;
            width: calc(100% + 8px);
            height: calc(100% + 8px);
            border: 2px solid #0ff;
            border-radius: 10px;
            opacity: 0;
            transition: all 0.3s ease;
        }

        .neon-button:before {
            transform: rotate(45deg);
        }

        .neon-button:hover:before,
        .neon-button:hover:after {
            opacity: 1;
            box-shadow: 0 0 40px #0ff, 0 0 80px #0ff, 0 0 120px #0ff;
        }
    </style>
</head>
<body>
    <a href="#" class="neon-button">Hi</a>
</body>
</html>

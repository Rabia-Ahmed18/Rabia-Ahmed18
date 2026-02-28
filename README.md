<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body { 
            background: #000; 
            color: #fff; 
            font-family: Arial, sans-serif; 
            overflow: hidden; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            height: 100vh;
        }

        .animated-wave {
            position: relative;
            width: 100%;
            height: 30px;
            background: linear-gradient(to right, #00f, #0ff);
            overflow: hidden;
            animation: wave 1.5s linear infinite;
        }

        @keyframes wave {
            0% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0); }
        }

        .typewriter {
            font-size: 2em;
            border-right: 0.15em solid orange;
            white-space: nowrap;
            overflow: hidden;
            animation: typing 4s steps(40, end) infinite;
            width: 22em;
            animation: typing 3.5s steps(30, end) infinite, blink-caret 0.75s step-end infinite;
        }

        @keyframes typing {
            from { width: 0; }
            to { width: 22em; }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent; }
            50% { border-color: orange; }
        }

        .bouncy {
            display: inline-block;
            animation: bounce 1s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-30px);
            }
            60% {
                transform: translateY(-15px);
            }
        }

        .gradient-text {
            background: linear-gradient(135deg, #f06, #a0f);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }

        .pulsing {
            display: inline-block;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
    </style>
    <title>Animated README</title>
</head>
<body>
    <div class="animated-wave"></div>
    <div class="typewriter">Welcome to my GitHub Repository!</div>
    <div class="bouncy">Check out my projects!</div>
    <div class="pulsing gradient-text">Enjoy the animations!</div>
</body>
</html>
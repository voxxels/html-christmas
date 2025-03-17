<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bubble Animation</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #121212;
            overflow: hidden;
        }
        .bubble {
            position: absolute;
            bottom: -100px;
            width: 50px;
            height: 50px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 50%;
            animation: rise 5s infinite;
        }
        @keyframes rise {
            0% {
                transform: translateY(0);
                opacity: 1;
            }
            100% {
                transform: translateY(-600px);
                opacity: 0;
            }
        }
    </style>
</head>
<body>

<div class="bubble" style="left: 30%; animation-delay: 0.5s;"></div>
<div class="bubble" style="left: 50%; animation-delay: 1s;"></div>
<div class="bubble" style="left: 70%; animation-delay: 1.5s;"></div>
<div class="bubble" style="left: 20%; animation-delay: 2s;"></div>
<div class="bubble" style="left: 80%; animation-delay: 2.5s;"></div>

</body>
</html>

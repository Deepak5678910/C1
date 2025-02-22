<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moving Nursing Notes with Ball</title>
    <style>
        /* Container for the moving text and ball */
        .container {
            position: relative;
            height: 200px;
            overflow: hidden;
        }

        /* Style for the nursing notes text */
        .nursing-notes {
            color: red;
            font-size: 24px;
            font-weight: bold;
            position: absolute;
            top: 50px;
            left: 0;
            animation: moveTextAndBall 5s linear infinite;
        }

        /* Style for the moving ball */
        .moving-ball {
            width: 50px;
            height: 50px;
            background-color: blue;
            border-radius: 50%;
            position: absolute;
            top: 100px;
            left: 0;
            animation: moveTextAndBall 5s linear infinite;
        }

        /* Animation for the text and ball */
        @keyframes moveTextAndBall {
            0% {
                left: 0;
            }
            50% {
                left: calc(100% - 100px);
            }
            100% {
                left: 0;
            }
        }
    </style>
</head>
<body>
    <!-- Container for the moving text and ball -->
    <div class="container">
        <!-- Nursing Notes Text -->
        <div class="nursing-notes">Nursing Notes</div>

        <!-- Moving Ball -->
        <div class="moving-ball"></div>
    </div>
</body>
</html>

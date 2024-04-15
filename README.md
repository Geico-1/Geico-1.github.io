# videogame
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.0/p5.min.js" integrity="sha512-uaz5GpnQoE6t5echKlX8P52czvsIGgLPcvlzfvRubLZ1Hp8JemUDnbUiAahbVtPb+jUVrNETuXvAhDDF/N3M4w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script> 
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@200&family=Pixelify+Sans:wght@400..700&family=Playpen+Sans:wght@200&display=swap" rel="stylesheet">
  
    <style>
        @keyframes startanimation {
            100% {
                font-size: 70px;
            }
        }
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            height: 100vh;
        }
        #TITLE {
            position: absolute;
            font-family: "Pixelify Sans", sans-serif;
            font-size: 125px;
        }
        #Clicky {
            position: absolute;
            font-family: "Pixelify Sans", sans-serif;
            font-size: 60px;
            top: 60vh;
            color: white;
            animation-name: startanimation;
            animation-duration: 2s;
            animation-iteration-count: infinite;
            animation-direction: alternate;
        }
    </style>
</head>
<body>
    <h1 id="TITLE">Dinosaur Quest</h1>
    <h2 id="Clicky">Click to Start</h2>
    <script>
        let background

        //create full size canvas. w and h will return the size in pixels of your width and height of the window WHEN THE PAGE LOADS
        //w and h are integers
        let w = window.innerWidth
        let h = window.innerHeight



        function preload() {
            background = loadImage('background.gif')
        }

        //Now I create my canvas
        function setup() {
            createCanvas(w,h)
        }

        function draw() {
            image(background,0,0,w,h)


            //if mouse is pressed then start the game
            if (mouseIsPressed === true) {
            window.location.href = 'tutorial.html'

        }
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Love</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffebf0;
            padding-top: 50px;
        }
        h1, h2 {
            color: #d63384;
        }
        #buttons, #flowerSection, #successPage, #tantrumPage, #finalConfirm, #letter {
            margin-top: 20px;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        #hi {
            background-color: #28a745;
            color: white;
        }
        #bye, #noFlower, #noSuccess, #rejectFinal {
            background-color: #dc3545;
            color: white;
        }
        #yesFlower, #yesSuccess, #yesTantrum, #acceptFinal {
            background-color: #ff69b4;
            color: white;
        }
        #flowerImage {
            display: none;
            margin-top: 20px;
            width: 200px;
            image-rendering: pixelated;
        }
        #letter {
            display: none;
            font-size: 18px;
            color: #333;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>

    <h1>Hi Wania Ur Rehman✨</h1>
    
    <div id="buttons">
        <button id="hi" class="btn" onclick="showFlowerSection()">Hi</button>
        <button id="bye" class="btn" onclick="growHi()">Bye</button>
    </div>

    <div id="flowerSection" style="display: none;">
        <h2>Accept these flowers? <br> <small>(Until I give real ones 🌷)</small></h2>
        <img id="flowerImage" src="https://i.imgur.com/YfJhbz8.png" alt="Pixelated Tulip Bouquet">
        <br>
        <button id="yesFlower" class="btn" onclick="showSuccessPage()">Yes</button>
        <button id="noFlower" class="btn" onclick="growYesFlower()">No</button>
    </div>

    <div id="successPage" style="display: none;">
        <h2>Will you be the reason behind all my success? <br> 
            <small>(Behind every successful man, there's a woman. But in my case, there's a shark 🦈.)</small>
        </h2>
        <button id="yesSuccess" class="btn" onclick="showTantrumPage()">Yes</button>
        <button id="noSuccess" class="btn" onclick="growYesSuccess()">No</button>
    </div>

    <div id="tantrumPage" style="display: none;">
        <h2>Can I get lifetime membership of your tantrums? ✨</h2>
        <button id="yesTantrum" class="btn" onclick="showFinalConfirm()">Yes</button>
        <button id="noTantrum" class="btn" onclick="fakeNoTantrum()">No</button>
    </div>

    <div id="finalConfirm" style="display: none;">
        <h2>Press Yes for my special words for you 💖<br> 
            <small>(Until I am confirmed enough to do everything in this world for you practically)</small>
        </h2>
        <button id="acceptFinal" class="btn" onclick="showLetter()">I Accept</button>
        <button id="rejectFinal" class="btn" onclick="growAcceptFinal()">Reject</button>
    </div>

    <div id="letter">
        <h2>My Dearest Love,</h2>
        <p>
             This might just be another letter for you, but for me its another time i am lucky enough to express myself. I never actually realized that valentines is something (cringe na khna) but today idkit felt like i have someone for this day about whom i can think and admire on this day. You are my first and IA the last love of my life. I really wanna be confirmed enough to start doing things for you. I want to see the smile on your face. You, Wania, have become everything for me and i wanna see us be permanent soon (plsss Allah jldi krein 😭 ). I'll always stay loyal to you hamesha. Your tantrums feels like the most precious and beautiful thing in the whole world. You're not difficult, you're the most beautiful and the most perfect girl i ever saw and i just want you.

        </p>
        <p>With all my love,</p>
        <p><strong>Talha</strong></p>
    </div>

    <script>
        function growHi() {
            let hiButton = document.getElementById("hi");
            let size = parseInt(hiButton.style.fontSize) || 20;
            size += 10;
            hiButton.style.fontSize = size + "px";
        }

        function showFlowerSection() {
            document.getElementById("flowerSection").style.display = "block";
            document.getElementById("hi").style.display = "none";
            document.getElementById("bye").style.display = "none";
        }

        function growYesFlower() {
            let yesFlower = document.getElementById("yesFlower");
            let size = parseInt(yesFlower.style.fontSize) || 20;
            size += 10;
            yesFlower.style.fontSize = size + "px";
        }

        function showSuccessPage() {
            document.getElementById("successPage").style.display = "block";
            document.getElementById("flowerSection").style.display = "none";
        }

        function growYesSuccess() {
            let yesSuccess = document.getElementById("yesSuccess");
            let size = parseInt(yesSuccess.style.fontSize) || 20;
            size += 10;
            yesSuccess.style.fontSize = size + "px";
        }

        function showTantrumPage() {
            document.getElementById("tantrumPage").style.display = "block";
            document.getElementById("successPage").style.display = "none";
        }

        function fakeNoTantrum() {
            alert("No button doesn't work! You have to say Yes 😉");
        }

        function showFinalConfirm() {
            document.getElementById("finalConfirm").style.display = "block";
            document.getElementById("tantrumPage").style.display = "none";
        }

        function growAcceptFinal() {
            let acceptFinal = document.getElementById("acceptFinal");
            let size = parseInt(acceptFinal.style.fontSize) || 20;
            size += 10;
            acceptFinal.style.fontSize = size + "px";
        }

        function showLetter() {
            document.getElementById("letter").style.display = "block";
            document.getElementById("finalConfirm").style.display = "none";
        }
    </script>

</body>
</html>

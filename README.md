<!doctype html>
<html lang="en">
<head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=divice-width, initial-scalee=1.0">
        <title> Emoji Changer</title>
        <style>
            body {
                display: flex;
                justify-content: center;
                align-items: center;
                height: 100vh;
                font-family: Arial, Helvetica, sans-serif;
                background-color: #f4f4f4;
                margin: 0;
            }
            #emoji {
                font-size: 100px;
                transition: transform 0.5s;
            }
        
        </style>
</head>
<body>
    
    <div id="Emoji">😀</div>

    <script>
        const emojis = ["😀", "😂", "😍", "😁", "😅", "🙂", "🙃", "🫠"] 
        const emojiElement = document.getElementById("emoji");

        function changeEmoji() {
            const randomindex = Math.floor(math.randome() * emojis.length);
        emojiElement.textcontent = emojis[randomindex];
        emojiElement.style.transform="scale(1.2)";
        setTimeout(() => emojiElement.style.transform = "scale(1)", 300);
        }

        // Change emoji every minute(60,000 milliseconds)
        setInterval(changeEmoji, 60000);

        //initial call to display the first emoji
        changeEmoji();
    </script>
</body>
</html>
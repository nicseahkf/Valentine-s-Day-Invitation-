# Valentine-s-Day-Invitation-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Invitation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            color: #d6336c;
            margin: 0;
            padding: 0;
        }
        .container {
            padding: 50px;
        }
        .invitation {
            display: none;
            font-size: 24px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            margin-top: 20px;
        }
        .reveal-button {
            padding: 10px 20px;
            font-size: 18px;
            color: white;
            background: #d6336c;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .reveal-button:hover {
            background: #b02a58;
        }
        .rsvp-buttons {
            margin-top: 20px;
        }
        .rsvp-button {
            padding: 10px 15px;
            font-size: 16px;
            color: white;
            background: #d6336c;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 5px;
        }
        .rsvp-button:hover {
            background: #b02a58;
        }
        .message {
            display: none;
            font-size: 20px;
            margin-top: 20px;
            background: white;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>You're Invited!</h1>
        <p>Join me for a special Valentine's Day celebration 💖</p>
        <button class="reveal-button" onclick="revealInvitation()">Click to Reveal</button>
        <div class="invitation" id="invitation">
            <p>🎉 Surprise! You're invited to our Valentine's Day date! 🎉</p>
            <p>📅 Date: February 14th</p>
            <p>📍 Location: Secret Romantic Venue</p>
            <p>💌 RSVP Now!</p>
            <div class="rsvp-buttons">
                <button class="rsvp-button" onclick="showMessage('yes')">Yes, I will attend</button>
                <button class="rsvp-button" onclick="showMessage('no')">No, I'm not free</button>
            </div>
        </div>
        <div class="message" id="yesMessage">
            <p>📍 A place where you can dive into the wonders of the ocean without getting wet, home to vibrant sea creatures and interactive exhibits—located near a famous waterfront or city landmark.</p>
        </div>
        <div class="message" id="noMessage">
            <p>🤔 Is it because it's not over 6 months?!</p>
        </div>
        <iframe style="margin-top:20px;" width="560" height="315" src="https://www.youtube.com/embed/fzQ6gRAEoy0?autoplay=1&loop=1&playlist=fzQ6gRAEoy0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
    
    <script>
        function revealInvitation() {
            document.getElementById("invitation").style.display = "block";
        }
        function showMessage(response) {
            document.getElementById("yesMessage").style.display = response === 'yes' ? 'block' : 'none';
            document.getElementById("noMessage").style.display = response === 'no' ? 'block' : 'none';
        }
    </script>
</body>
</html>

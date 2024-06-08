# <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Search Button</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: url('https://i.pinimg.com/originals/3b/eb/8e/3beb8eb2cc9939e5745d773ae3fd24f3.gif') no-repeat center center fixed;
            background-size: cover;
            font-family: Arial, sans-serif;
        }

        .container {
            text-align: center;
            position: relative;
            left: 10px; /* Move the container a little to the left */
        }

        #topImage {
            width: 600px;  /* Increase the size as needed */
            height: auto;  /* Auto height to maintain aspect ratio */
            margin-bottom: 50px;
        }

        #searchButton {
            background: none;
            border: none;
            padding: 0;
            cursor: pointer;
            outline: none;
            position: relative;
            left: -350px; /* Adjust to move the button to the right */
            top: -75px;  /* Move the button up */
        }

        #searchButton img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
        }

        .search-bar {
            display: none;
            position: absolute;
            bottom: 130%;
            left: 50%;
            transform: translateX(-50%);
            width: 320px;
            padding: 10px 20px;
            background-color: #fff;
            border: 2px solid #4caf50;
            border-radius: 25px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .search-bar input {
            width: 100%;
            padding: 10px;
            border: none;
            outline: none;
            font-size: 16px;
            border-radius: 20px;
            background-color: #f0f0f0;
        }

        .search-bar input:focus {
            background-color: #fff;
            box-shadow: 0 0 10px rgba(56, 142, 60, 0.3);
        }

        .right-side {
            position: absolute;
            top: 20px;
            right: 20px;
        }

        .left-side {
            position: absolute;
            top: 20px;
            left: 20px;
        }
        
        .widget-container {
            position: absolute;
            top: 20px;
            left: 0; /* Positioning to the left edge of the screen */
        }
    </style>
</head>
<body>
    <div class="widget-container">
        <script src="https://cdn.jsdelivr.net/npm/@widgetbot/crate@3" async defer>
            new Crate({
                server: '1248778916005412937', // RSProxies
                channel: '1248778916005412940' // #general
            })
        </script>
    </div>
    <div class="container">
        <img id="topImage" src="https://i.imgur.com/LIsqifi_d.webp?maxwidth=760&fidelity=grand" alt="Top Image">
        <button id="searchButton">
            <img src="https://i.imgur.com/24KAhcN_d.webp?maxwidth=760&fidelity=grand" alt="Search">
        </button>
        <div id="searchBar" class="search-bar">
            <input type="text" placeholder="Search...">
        </div>
    </div>
    <div class="right-side">
        <script>
            window.aichatbotApiKey = "b23ad20c-e5ad-4053-83bb-8436e8dc4276";
            window.aichatbotProviderId = "f9e9c5e4-6d1a-4b8c-8d3f-3f9e9c5e46d1";
        </script>
        <script src="https://script.chatlab.com/aichatbot.js" id="b23ad20c-e5ad-4053-83bb-8436e8dc4276" defer></script>
    </div>
    <script>
        document.getElementById('searchButton').addEventListener('click', function() {
            var searchBar = document.getElementById('searchBar');
            searchBar.style.display = 'block';
            this.style.display = 'none';  // Hide the button
        });
    </script>
</body>
</html>

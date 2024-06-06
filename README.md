<!DOCTYPE html>
<html>
<head>
    <title>My Firefox Start Page</title>
    <style>
        body {
            background-color: #111;
            color: #eee;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0 auto;
            max-width: 800px;
        }
        .links {
            margin-top: 20px;
        }
        .links a {
            color: #eee;
            text-decoration: none;
            margin: 0 10px;
            font-size: 18px;
            transition: all 0.3s ease;
        }
        .links a:hover {
            color: #888;
        }
        .clock {
            font-size: 24px;
            margin-top: 20px;
        }
        .search {
            margin-top: 20px;
        }
        .search input[type="text"] {
            padding: 10px;
            font-size: 16px;
            width: 600px;
            border-radius: 5px;
            border: none;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .search input[type="submit"] {
            padding: 10px;
            font-size: 16px;
            background-color: #222;
            color: #eee;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .search input[type="submit"]:hover {
            background-color: #444;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome back, user!</h1>
        <div class="clock">
            <span id="time"></span>
        </div>
        <div class="links">
            <a href="https://hurawatch2.to">HuraWatch2</a>
            <a href="https://anix.to">Anix</a>
            <a href="https://mangafire.to">MangaFire</a>
            <a href="https://www.youtube.com">YouTube</a>
            <a href="https://www.reddit.com">Reddit</a>
            <a href="https://huggingface.co/chat/">HuggingFace</a>
        </div>
        <div class="search">
            <form action="https://duckduckgo.com/" target="_blank">
                <input type="text" name="q" placeholder="Search...">
                <input type="submit" value="DuckDuckGo">
            </form>
        </div>
    </div>
    <script>
        // Update the clock every second
        setInterval(function() {
            var now = new Date();
            var time = now.toLocaleTimeString('en-US', {timeZone: 'America/Toronto'});
            document.getElementById('time').textContent = time;
        }, 1000);
    </script>
</body>
</html>

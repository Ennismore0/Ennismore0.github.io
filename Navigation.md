<title>Ennismore0 | Navigation</title>
<h2>Navigation</h2>

<a href="Mods/Mods.html">Mods I've Made</a>
<br>
<br>
<a href="About/Activities.html">Other things I do</a>
<br>
<br>
<a href="About/Other/OtherStuff.html">Non-Minecraft!</a>
<br>
<br>
<br>
<a href="README.md">Home</a>

<body>
    <script>
        // Create a broadcast channel (same name across tabs)
        const channel = new BroadcastChannel('console_broadcast');

        // Listen for messages from other tabs
        channel.onmessage = (event) => {
            console.log("Received from another tab:", event.data);
        };

        // Automatically send the broadcast message
        channel.postMessage("wowowow");
        console.log("Hey, I see you looking at the console, you little detective! While I have your attention, I may as well congratulate you! ;D ");
    </script>
</body>

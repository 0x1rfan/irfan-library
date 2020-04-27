
<!DOCTYPE html>
<html>
    <head>
        <title>Owl Hub</title>

        <meta charset = "utf-8">
		<link rel = "shortcut icon" type = "image/x-icon" href="Logo.ico" />

		<meta name = "author" content = "Owl Hub" />
		<meta name = "description" content = "Owl Hub" />
		<meta name = "keywords" content = "Owl, Hub, OwlHub, script, lua, krnl" />

		<meta property = "og:title" content = "Owl Hub" />
		<meta property = "og:description" content = "Official website for Owl Hub" />
		<meta property = "og:type" content = "website" />
		<meta property = "og:url" content = "https://owlhub.ga" />
		<meta property = "og:secure_url" content = "https://owlhub.ga">
		<meta property = "og:image" content = "https://owlhub.ga/Logo.ico" />

        <style>
            body {
				background-color: rgb(25, 25, 25);
                color: white;
                font-family: "Trebuchet MS";
			}

            body::-webkit-scrollbar {
                width: 12px;
            }
      
            body::-webkit-scrollbar-thumb {
                background-color: rgb(80, 80, 80);
            }

            #gamesLabel {
                background-color: rgb(25, 25, 25); 
                color: rgb(255, 255, 255);
                border: 0px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <center>
            <h4 id="gamesLabel"></h20>
            <br>
            <br>
        </center>

        <script type="text/javascript">
            const gamesBox = document.getElementById("gamesLabel");

            const games = new XMLHttpRequest();
            const gamesURL = "https://crishoux.github.io/OwlHub/Games.txt";
            games.open("GET", gamesURL, true);
            games.send();

            games.onreadystatechange = () => {
                gamesBox.innerText = games.responseText;
            }
        </script>
    </body>
</html>

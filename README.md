<html>

<head>
	<title>Thanksgiving Match Game</title>

	<link href="https://fonts.googleapis.com/css2?family=Sniglet&display=swap" rel="stylesheet">
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
	<script type="text/javascript" src="logic.js"></script>
	<link rel="stylesheet" href="style.css">

	<style>
		
		
        body {
		   background-image: URL('autumn.jpg');
		   background-size: 50%;
		   text-align: center;
		}
		
		h1 {
		  font-family: 'Sniglet', cursive;
		  color: orange;
		}
		
		#game-wrapper {
		 margin: auto;
		 margin-top: 40px;
		 padding: 20px;
		 width: 760px;
		 background-color: white;
		 border-radius: 20px;
		 border: 5px solid orange;
		}
		
		.card {
		 position: absolute;
		 height:100%;
		 width:100%;
		 backface-visibility: hidden;
		}
		
		.card_front {
			background: linear-gradient(yellow, orange);
		}
		
		.card_back {
			background-color: white;
			transform: rotateY(180deg);
		}
		.card_back img {
			width: 80px;
			height: 80px;
			margin-top: 10px;
		}
				.is-flipped {
			transform: rotateY(180deg);
		}
				a {
			font-family: 'Sniglet', cursive;
			background-color: orange;
			display: block;
			padding: 10px;
			margin: 10px;
		}
	</style>
</head>

<body>


	<div id="game-wrapper"> 
	<h1>Thanksgiving Card Game</h1>
	<a onclick="start()">RESTART</a>
	<div id="match-grid"></div>
	</div>


	<script>
		var images = ["pumpkin.png", "boat.png", "corn.png"];

		start();

	</script>
</body>

</html>

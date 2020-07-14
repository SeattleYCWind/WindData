<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

<link rel="stylesheet" type="text/css" href="mystyles.css">

<html lang="en">

<head>
    <title>SYC Outstation Winds</title>
    <!meta http-equiv="refresh" content="600;url=ftp://ftp-americas.ausenco.com/100686-01/web/index.html">
</head>

<body>
	<canvas id="myCanvas" width="584" height="122";"></canvas>

	<script>
	var c = document.getElementById("myCanvas");
	var ctx = c.getContext("2d");

	// Create gradient
	var grd = ctx.createLinearGradient(0,0,584,0);
	grd.addColorStop(0,"#000077");
	grd.addColorStop(1,"#999999");

	// Fill with gradient
	ctx.fillStyle = grd;
	ctx.fillRect(0,0,584,122);

	// Draw logo
   	var img = new Image();
	img.onload = function() {
   		ctx.drawImage(img,240,0);
	};
	img.src = "SYClogonew.png";
	</script>

	<body style="background-color:black;">

    <!img src="SYClogonew.png?random=<?php echo rand() ?" alt="Sig">

    <h1>Wind Speed and Direction at SYC Outstations</h1>

    <hr size="3" width="582" align="left" noshade>

    <h2>Garden Bay, Sunshine Coast, British Columbia</h2>
    <h2>49.6292 deg N, 124.0195 deg W (<a href="https://www.google.ca/maps/place/49%C2%B037'45.3%22N+124%C2%B001'09.9%22W/@49.6229204,-124.0380638,10.5z/data=!4m5!3m4!1s0x0:0x0!8m2!3d49.6292429!4d-124.0194232" target="_blank">map</a>)</h2>
    <h3>Latest measurements<h3>

    <hr size="3" width="582" align="left" noshade>

    <!script src="wind.js"></script>

    <p>Copyright 2015 Ausenco</p>

</body>

</html>

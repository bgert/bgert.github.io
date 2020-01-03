---
layout: null
title: don't click me
permalink: /clickme/
---
<html>
	<head>
		<!-- Latest compiled and minified CSS -->
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">

		<!-- jQuery library -->
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

		<!-- Latest compiled JavaScript -->
		<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
	</head>
	<body>
		<div class="container">
			<button type="button" class="btn btn-outline-success" id="bjutton">
				Click Me! ( ͡~ ͜ʖ ͡°)
			</button>
		</div>
	</body>
	<script>
		$('#bjutton').on('mouseenter',function(e){
	    var maxX = $(window).width() - $(this).width();
	    var maxY = $(window).height() - $(this).height();
	    $(this).css({
	        'left':getRandomInt(0, maxX),
	        'top':getRandomInt(0, maxY)
	    });
		});
		function getRandomInt(min, max) {
		    return Math.floor(Math.random() * (max - min + 1)) + min;
		}
	</script>
</html>

<style type="text/css">
	#bjutton {
	position:absolute;
    border: 1px solid red;
    height:50px;
}
	</style>

---
layout: slides
title: Slide
permalink: /slider/
---
<html>
	<head>
		<!-- toss in our stylesheet -->
		<link rel="stylesheet" href="../css/style.css" type="text/css" media="screen" />
		

	</head>
	<body>
		
		<!-- add previous/next links.... 
		<a href="#" class="unslider-arrow prev">Previous slide</a>
		<a href="#" class="unslider-arrow next">Next slide</a> -->
		
		<div class="banner">
			<ul>
				<!-- external links....
				<li style="background-image: ../images/image1.jpg;"></li> -->
			
				<!-- internal links... -->
				
	  	    		<li><img src=" ../images/image1.jpg" /> </li>
	  	    		<li><img src=" ../images/image2.jpg "/> </li>
	  	    		<li><img src=" ../images/image3.jpg "/> </li>
	  	    		<li><img src=" ../images/image4.jpg "/> </li>
			</ul>
		</div>
	
	    <!-- pull in the js code -->
	
		<script src="http://code.jquery.com/jquery-latest.min.js"></script>
		<script src="http://unslider.com/unslider.min.js"></script>
		
		<!-- previous/next links -->
	    <!--	<script>
		    var unslider = $('.banner').unslider();

		    $('.unslider-arrow').click(function() {
		        var fn = this.className.split(' ')[1];

		        //  Either do unslider.data('unslider').next() or .prev() depending on the className
		        unslider.data('unslider')[fn]();
		    });
		</script> -->
		
		<script>
			$(document).ready(function(){
				$('.banner').unslider({
					speed: 500,               //  The speed to animate each slide (in milliseconds)
					delay: 3000,              //  The delay between slide animations (in milliseconds)
					complete: function() {},  //  A function that gets called after every slide animation
					keys: true,               //  Enable keyboard (left, right) arrow shortcuts
					dots: true,               //  Display dot navigation
					fluid: false              //  Support responsive design. May break non-responsive designs
				});
			});
		</script>
	</body>
</html>







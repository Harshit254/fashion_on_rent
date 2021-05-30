# fashion_on_rent
# it is e-commerce website which provides fashion on rent 
<?php

session_start();
if(!isset($_SESSION['username']))
{
	header('location:loginpage.php');
}


?>


<!DOCTYPE html>
<html>
	<title>FASHION ON RENT</title>
	<link rel="stylesheet" type="text/css" href="myntras.css">
	<script src="https://kit.fontawesome.com/d2305cdb4a.js" crossorigin="anonymous"></script>
	<script type="text/javascript" src="js.js"></script>
	<link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@600&display=swap" rel="stylesheet">
	<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
</head>
<body>
	<div class="navigation" id="navigationbar">
		<div class="logo" id="myntralogo">
			<img src="designer.jpg" alt="myntralogo">
		</div>
		<nav>
			<div class="category" id="categoryname">
				<div class="dropdown">
					<a href="myntra.html" class="do">men</a>
					<!--FOR MENS SECTIION-->
					<div class="men" id="mens">
						<div class="menswear">
							<ul>
								<li><a href="#">GROOM WEAR</a></li>
								<li><a href="">FORMALS</a></li>
								<li><a href="#">DESIGNER WEAR</a></li>
								<li><a href="#">DESIGNERS</a></li>
								<li><a href="#">ACCESSORIES</a></li>
							</ul>
						</div>
					</div>
				</div>
				<!--end-->

				<div class="dropdown2">
					<a href="table.html" onmouseenter="female()" class="do">women</a>
					<!--female section start-->
					<!-- FOR FEMALE SECTION-->
					<div class="female" id="females" onmouseleave="female2()">
						<div class="femalewear">
							<ul>
								<li><a href="#">BRIDAL WEAR</a></li>
								<li><a href="">FORMALS</a></li>
								<li><a href="#">DESIGNER WEAR</a></li>
								<li><a href="#">SAREES</a></li>
								<li><a href="#">DESIGNERS</a></li>
								<li><a href="#">ACCESSORIES</a></li>
							</ul>
							
						</div>
					</div>
				</div>
				<!--end of female-->
				<div class="dropdown3">
					<a href="table.html">kids</a>
					<!--for kids-->
					<!--FOR home and living-->
					<div class="kid" id="kids">
						<div class="kidswear">
							<ul>
								<li><a href="#">FANCY DRESSES</a></li>
								<li><a href="">TOP DESIGNED</a></li>
								<li><a href="#">DESIGNERS</a></li>
								<li><a href="#">ACCESSORIES</a></li>
							</ul>
						</div>
					</div>
				</div>
				<!---->
				<div class="dropdown4">
					<a href="table.html">ACCESSORIES</a>
					<!--home & living-->
					<!--FOR KIDS-->
					<div class="homeandliving" id="kids">
						<div class="accessories">
							<ul>
								<li><a href="#">JEWELLERIES</a></li>
								<li><a href="">SUN GLASSES</a></li>
								<li><a href="#">WATCHES</a></li>
								<li><a href="#">CAMERAS</a></li>
								<li><a href="#"></a></li>
							</ul>
						</div>
					</div>
				</div>
				<!---->
			</nav>
			<div class="search" id="searchbar">
				<input type="text" name="searchbar" placeholder="Search for Product,Brand and More" >
				<i class="fas fa-search"></i>
			</div>
			<div class="profile" id="profilename">
				<div class="profilelogo">
					<div class="searching">
						<i class="far fa-user"></i>
					</div>
				</div>
				<div class="profiletext">
					<a href="#">profile</a>
				</div>
				<div class="login">
					<h5>welcome</h5>
					<h5><?php echo $_SESSION['username'];?></h5>
					<p>To Access Account Login Your Account</p>
					<a href="loginpage.php" style="color: white; text-decoration: none;">Login</a>
					<a href="logout.php" style="color: white; text-decoration: none;">logout</a>
					<hr>
					<ul>
						<li><a href="#">Orders</a></li>
						<li><a href="">Wishlist</a></li>
						<li><a href="#">Coupons</a></li>
						<li><a href="#">Gift Card</a></li>
						<li><a href="#">Contact Us</a></li>
					</ul>

				</div>
			</div>
			<div class="wishlist" id="wishlistname">
				<div class="wishlistlogo">
					<img src="wishlist.png">
				</div>
				<div class="wishlisttext">
					<p>wishlist</p>
				</div>
			</div>
			<div class="bag" id="shoppingcart">
				<div class="baglogo">
					<i class="fas fa-shopping-bag"></i>
				</div>
				<div class="bagtext">
					<a href="cart.html" style="color: black; text-decoration: none;">bag</a>
				</div>
			</div>
		</div>
	</div></nav></div>
	<div class="slideshow middle">
		<div class="slides">
			<input type="radio" name="r" id="r1" checked>
			<input type="radio" name="r" id="r2">
			<input type="radio" name="r" id="r3">
			<input type="radio" name="r" id="r4">
			<input type="radio" name="r" id="r5">
			<div class="slide">
				<img src="virat1.jpg.png">
			</div>
			<div class="slide s1">
				<img src="marriage2.png">
			</div>
			<div class="slide">
				<img src="131.png">
			</div>
			<div class="slide">
				<img src="4.jpg">
			</div>
			<div class="slide">
				<img src="141.png">
			</div>
			<div class="navigation-auto">
				<div class="auto-btn1"></div>
				<div class="auto-btn2"></div>
				<div class="auto-btn3"></div>
				<div class="auto-btn4"></div>
				<div class="auto-btn5"></div>
			</div>
		</div>
		<div class="navi">
			<label for="r1" class="bar"></label>
			<label for="r2" class="bar"></label>
			<label for="r3" class="bar"></label>
			<label for="r4" class="bar"></label>
			<label for="r5" class="bar"></label>
		</div>
	</div>

	<!--<div class="slider">
		<div class="slides">
			<input type="radio" name="r" id="r1" checked>
			<input type="radio" name="r" id="r2">
			<input type="radio" name="r" id="r3">
			<input type="radio" name="r" id="r4">
			<input type="radio" name="r" id="r5">

			<div class="slide first">
				<img src="1.jpg">
			</div>
			<div class="slide second">
				<img src="2.jpg">
			</div>
			<div class="slide third">
				<img src="3.jpg">
			</div>
			<div class="slide fourth">
				<img src="4.jpg">
			</div>
			<div class="slide fifth">
				<img src="girls.jpg">
			</div>

			<div class="navigation-auto">
				<div class="auto-btn1"></div>
				<div class="auto-btn2"></div>
				<div class="auto-btn3"></div>
				<div class="auto-btn4"></div>
				<div class="auto-btn5"></div>
			</div>

		</div>
		<div class="navigation-manual">
			<label for="r1" class="manual-btn"></label>
			<label for="r2" class="manual-btn"></label>
			<label for="r3" class="manual-btn"></label>
			<label for="r4" class="manual-btn"></label>
			<label for="r5" class="manual-btn"></label>
		</div>
	</div>-->
	<script type="text/javascript">
		var counter =1;
		setInterval(function(){
			document.getElementById('r' + counter).checked = true;
			counter++;
			if(counter>5)
			{
				counter=1;
			}
		},5000);
	</script>


	<!--designers-->


	<div class="designer">
		<div class="names"><p>#SHOP&nbsp; BY&nbsp; TOP&nbsp; DESIGNERS</p></div>
		<div class="designername">
			<div class="sabyasacchi" id="1">
				<img src="sabyasacchi.jpg">
				<p class="name">Sabyasacchi Mukherjee</p>
			</div>
			<div class="sabyasacchi" id="2">
				<img src="manish.jpg">
				<p class="name">Manish Manhotra</p>
			</div>
			<div class="sabyasacchi" id="3">
				<img src="khan.jpg">
				<p class="name">Naeem Khan</p>
			</div>
			<div class="sabyasacchi 3" id="4">
				<img src="neeta.jpg">
				<p class="name">Neeta Nulla</p>
			</div>
			<div class="sabyasacchi 4" id="5">
				<img src="tarun.jpg">
				<p class="name">Tarun Tahiliani</p>
			</div>
			
		</div>
   </div>



   <!--ethnic wears-->



   <div class="ethnicwear">
		<div class="names"><p>#WEDDING&nbsp;  OUTFITS &nbsp; BY &nbsp; REGION</p></div>
		<div class="ethnicweartype">
			<div class="sabyasacchi" id="1">
				<img src="northindian.jpg">
				<p class="name">north indian</p>
			</div>
			<div class="sabyasacchi" id="2">
				<img src="southindian1.jpg">
				<p class="name">south indian</p>
			</div>
			<div class="sabyasacchi" id="3">
				<img src="westindian.jpg">
				<p class="name">west indian</p>
			</div>
			<div class="sabyasacchi 3" id="4">
				<img src="eastindian.jpg">
				<p class="name">east indian</p>
			</div>
			
		</div>
   </div>


   <!--traditional-->


   <div class="traditional">
		<div class="names"><p>#TRADITIONAL</p></div>
		<div class="traditionaltype">
			<div class="sabyasacchi" id="1">
				<img src="muslim.jpg">
				<p class="name">salwar kameez</p>
			</div>
			<div class="sabyasacchi" id="2">
				<img src="saree.jpeg">
				<p class="name">saree</p>
			</div>
			<div class="sabyasacchi" id="3">
				<img src="lehga.jpg">
				<p class="name">lehnga</p>
			</div>
			<div class="sabyasacchi 3" id="4">
				<img src="sherwani.jpeg">
				<p class="name">sherwani</p>
			</div>
			<div class="sabyasacchi 4" id="5">
				<img src="pathansuit.jpg">
				<p class="name">pathan suit</p>
			</div>
		</div>
   </div>

   <!--westernwear-->


   <div class="westernwear">
		<div class="names"><p>#WESTERN WEAR</p></div>
		<div class="westerntype">
			<div class="sabyasacchi" id="1">
				<img src="western1.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi" id="2">
				<img src="western2.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi" id="3">
				<img src="western3.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi 3" id="4">
				<img src="western4.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi 4" id="5">
				<img src="western5.jpg">
				<p class="name">rent now</p>
			</div>
		</div>
   </div>


   <!--top accessories-->


   <div class="accesories">
		<div class="names"><p>#ACCESSORIES</p></div>
		<div class="topaccesories">
			<div class="sabyasacchi" id="1">
				<img src="watches.jpg">
				<p class="name">watches</p>
			</div>
			<div class="sabyasacchi" id="2">
				<img src="sunglass.jpg">
				<p class="name">sun glasses</p>
			</div>
			<div class="sabyasacchi" id="3">
				<img src="western3.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi 3" id="4">
				<img src="western4.jpg">
				<p class="name">rent now</p>
			</div>
			<div class="sabyasacchi 4" id="5">
				<img src="western5.jpg">
				<p class="name">rent now</p>
			</div>
		</div>
   </div>

<!--footer-->
  
   	<div class="containertag">
   		<div class="onlineshopping">
   			<h3>ONLINE SHOPPING</h3>
   			<UL>
   				<li>men</li>
   				<li>women</li>
   				<li>kids</li>
   				<li>accessories</li>
   			</UL>
   		</div>
   		<div class="usefullinks">
   			<h3> useful links</h3>
   			<ul>
   				<li><a href ="contact.php" style="color: white; text-decoration: none;">contact us</a></li>
   				<li>FAQ</li>
   				<li>T&C</li>
   				<li>terms of use</li>
   				<li>traking order</li>
   				<li>shipping</li>
   				<li>cancellation</li>
   				<li>returns</li>
   				<li>white hat</li>
   				<li>blog</li>
   				<li>career</li>
   				<li>privacy policy</li>
   				<li>site map</li>
   			</ul>
   		</div>
   		<div class="keep">
   			<h3>keep in touch</h3>
   			<div><i class="fab fa-instagram"></i></div>
   			<div><i class="fab fa-facebook-square"></i></div>
   			<div><i class="fab fa-twitter"></i></div>
   			<div><i class="fab fa-youtube"></i></div>
   		</div>
   		<div class="thapa">
   			<div class="original">
   				<div><img src="original.png"></div>
   				<div><p>100% original</p></div>
   			</div>
   			<div class="return">
   				<div><i class="fas fa-exchange-alt"></i></div>
   				<div><p>easy returns</p></div>
   			</div>
   			<div class="delivery">
   				<div><i class="fas fa-truck"></i></div>
   				<div><p>fast delivery</p></div>
   			</div>


   		</div>
   	</div>
  



		

	
</body>
</html>

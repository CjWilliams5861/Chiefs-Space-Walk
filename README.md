FOR HOME PAGE=

Home.html


<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Custom Website</title>
	<link rel="stylesheet" href="Home.css">
</head>
<body>
	<div class="wrapper">
			<nav class="navbar">
				<img class="logo" src="logo.png">
				<ul>
					<li><a class="active" href="#">Home</a></li>
					<li><a href="#">About</a></li>
					<li><a href="#">Services</a></li>
					<li><a href="../Contact/Contact.html">Contact</a></li>
					<li><a href="#">Feedback</a></li>
				</ul>
			</nav>
			<div class="center">
			<h1>Welcome To Chiefs Laboratory</h1>
			<h2>Create Something Guided</h2>
			<div class="buttons">
			<button>Explore More</button>
			<button class="btn2">Subscribe Us</button>
		</div>
		</div>
</body>
</html>
Home.css

@import url("https://fonts.googleapis.com/css?family=Roboto:700&display=swap");
* {
  padding: 0;
  margin: 0;
}
.wrapper {
  background: url(sun.jpg) no-repeat;
  background-size: cover;
  height: 100vh;
}
.navbar {
  position: fixed;
  height: 80px;
  width: 100%;
  top: 0;
  left: 0;
  background: rgba(0, 0, 0, 0.4);
}
.navbar .logo {
  width: 140px;
  height: auto;
  padding: 20px 100px;
}
.navbar ul {
  float: right;
  margin-right: 20px;
}
.navbar ul li {
  list-style: none;
  margin: 0 8px;
  display: inline-block;
  line-height: 80px;
}
.navbar ul li a {
  font-size: 20px;
  font-family: "Roboto", sans-serif;
  color: white;
  padding: 6px 13px;
  text-decoration: none;
  transition: 0.4s;
}
.navbar ul li a.active,
.navbar ul li a:hover {
  background: red;
  border-radius: 2px;
}
.wrapper .center {
  position: absolute;
  left: 50%;
  top: 55%;
  transform: translate(-50%, -50%);
  font-family: sans-serif;
  user-select: none;
}
.center h1 {
  color: white;
  font-size: 70px;
  width: 900px;
  font-weight: bold;
  text-align: center;
}
.center h2 {
  color: white;
  font-size: 70px;
  font-weight: bold;
  margin-top: 10px;
  width: 885px;
  text-align: center;
}
.center .buttons {
  margin: 35px 280px;
}
.buttons button {
  height: 50px;
  width: 150px;
  font-size: 18px;
  font-weight: 600;
  color: #ffb3b3;
  background: red;
  outline: none;
  cursor: pointer;
  border: 1px solid #cc0000;
  border-radius: 25px;
  transition: 0.4s;
}
.buttons .btn2 {
  margin-left: 25px;
}
.buttons button:hover {
  background: #cc0000;
}

contact.html

<!DOCTYPE html>
<html>
<head>
	<title>Contact us</title>
	<link rel="stylesheet" type="text/css" href="Contact.css">
	<link href="https://fonts.googleapis.com/css?family=Quicksand&display=swap" rel="stylesheet">
	<meta name="viewport" content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0">
</head>
<body>
	<div class="container">
		<div class="contact-box">
			<div class="left"></div>
			<div class="right">
				<h2>Contact Us</h2>
				<input type="text" class="field" placeholder="Your Name">
				<input type="text" class="field" placeholder="Your Email">
				<input type="text" class="field" placeholder="Phone">
				<textarea placeholder="Message" class="field"></textarea>
				<button class="btn">Send</button>
			</div>
		</div>
	</div>
</body>
</html>
contact.css

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Quicksand", sans-serif;
}

body {
  height: 100vh;
  width: 100%;
}

.container {
  position: relative;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px 100px;
}

.container:after {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  background: url("./bg.jpg") no-repeat center;
  background-size: cover;
  filter: blur(50px);
  z-index: -1;
}
.contact-box {
  max-width: 850px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #fff;
  box-shadow: 0px 0px 19px 5px rgba(0, 0, 0, 0.19);
}

.left {
  background: url("./phn.jpg") no-repeat center;
  background-size: cover;
  height: 100%;
}

.right {
  padding: 25px 40px;
}

h2 {
  position: relative;
  padding: 0 0 10px;
  margin-bottom: 10px;
}

h2:after {
  content: "";
  position: absolute;
  left: 50%;
  bottom: 0;
  transform: translateX(-50%);
  height: 4px;
  width: 50px;
  border-radius: 2px;
  background-color: #2ecc71;
}

.field {
  width: 100%;
  border: 2px solid rgba(0, 0, 0, 0);
  outline: none;
  background-color: rgba(230, 230, 230, 0.6);
  padding: 0.5rem 1rem;
  font-size: 1.1rem;
  margin-bottom: 22px;
  transition: 0.3s;
}

.field:hover {
  background-color: rgba(0, 0, 0, 0.1);
}

textarea {
  min-height: 150px;
}

.btn {
  width: 100%;
  padding: 0.5rem 1rem;
  background-color: #2ecc71;
  color: #fff;
  font-size: 1.1rem;
  border: none;
  outline: none;
  cursor: pointer;
  transition: 0.3s;
}

.btn:hover {
  background-color: #27ae60;
}

.field:focus {
  border: 2px solid rgba(30, 85, 250, 0.47);
  background-color: #fff;
}

@media screen and (max-width: 880px) {
  .contact-box {
    grid-template-columns: 1fr;
  }
  .left {
    height: 200px;
  }
}HTML Code:

<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="utf-8">

<title>

Biography

</title>

<link rel="stylesheet" href="style.css">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

</head>

<body>

<section id="header">

<div class="container">

<img src="Img/logo.PNG" class="logo">

<div class="head-text">

<h1>CHIEF WILLIAMS TO MY Instructor I Am Mr.Williams aka Carl

<br>FTCC BABY!!!</h1>

<span class="square"></span>

<p>

HATS OFF TO MR NORRIS. Thank you

</p>

<br>

<button class="common-btn">GET STARTED</button>

</div>

</div>

</section>

<nav id="sidenav">

<ul>

<li><a href="#" >HOME</a></li>

<li><a href="#" >Bio</a></li>

<li><a href="#" >Results</a></li>

<li><a href="#" >Contact</a></li>

<li><a href="#" >OTHER</a></li>

</ul>

</nav>

<img src="Img/menu.png" id="menubtn">


<!--About Us-->


<section id="about">

<div class="about-left">

<img src="Img/similar1.jpg">

</div>

<div class="about-right">


<div class="about-text">

<h2>

Family

I have 1 brother and one sister we live together.

</h2>

<span class="square"></span>

<br>

<p1>

Wake County Is Home For Now

</p1><br>

<br>

<button class="common-btn">KEEP YOUR USERS</button>

</div>

</div>

</section>




<!--Hobbies-->


<section id="opration">

<div class="opration-row">

<img src="Img/opration.jpg">

</div>


<div class="opra-b-shadow">

<div class="opra-col">

<h3>

ALL hobbies

</h3>

<br>

<br>

<ul>

<li>

Reading

</li>

<br>

<li>

Football

</li>

<br>

<li>

Playing Games

</li>

<br>

<li>

Treking

</li>

<br>

</ul>

<button class="common-btn">KEEP YOUR USERS</button>

</div>

<br>

</div>

</section>

<!--Features-->


<section id="features">

<div class="fetures-row">

<div class="featues-col">

<img src="Img/setup1.PNG">

<h4>SETUP</h4>

<br>

<p2>

MR Norris CTI 110  Class is The reason i cancled my Transfer.

</p2>

</div>

<div class="featues-col">

<img src="Img/CODE.PNG">

<h4>Plans For Life?</h4>

<br>

<p2>

Computer Science and Web Development is Life!

</p2>

</div>

<div class="featues-col">

<img src="Img/START.PNG">

<h4>START&End Date.</h4>

<br>

<p2>

OCT.2022 & Dec.2022

</p2>

</div>

</div>

<div class="feature-btn">

<button class="common-btn">Start Setup</button>

</div>


</section>



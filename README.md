<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
<style media="screen">
	* {
    box-sizing: border-box;}
	
	.container{
		width:1020px;
		margin:3px auto;
	}
.flex-container {
  display: flex;
  flex-flow: wrap;
  align-items: stretch;
  background-color: orange;
}

.flex-container > div{
  background-color: magenta;
  color: white;
  margin: 10px;
  font-size: 30px;
  padding: 0 20px 0 20px;
  flex-direction: column;
}
	@media (max-width: 800px) {
  .flex-container {
    flex-direction: column;
	  background-color: yellow;
		}
	}
header{
  width:100%;
  height:70px;
  background-color:yellowgreen;
}
footer{
  width:100%;
  height:50px;
  background-color:yellowgreen;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  border: 1px solid #e7e7e7;
  background-color: yellow;
}

li {
  float: left;
}

li a {
  display: block;
  color: #666;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #ddd;
}

li a.active {
  color: white;
  background-color: #04AA6D;
}
	}
	@media (max-width: 1019px){
		.container{width:90%;}
		
		.makeMeStack{
			flex:100%;
		}
	}
</style>
	  <link rel="stylesheet" href="https://code.jquery.com/ui/1.13.3/themes/base/jquery-ui.css">
  <link rel="stylesheet" href="/resources/demos/style.css">
  <script src="https://code.jquery.com/jquery-3.7.1.js"></script>
  <script src="https://code.jquery.com/ui/1.13.3/jquery-ui.js"></script>
  <script>
  $( function() {
    $( "#accordion" ).accordion();
  } );
  </script>
  </head>
	<body>
    <div class="container">
<header>Flexbox Assignment</header>
<ul>
  <li><a class="active" href="#home">HOME</a></li>
  <li><a href="#skincare">SKINCARE</a></li>
  <li><a href="#shop">SHOP</a></li>
  <li><a href="#about">ABOUT ME</a></li>
</ul>
		
<div class="flex-container">
	<div class="makeMeStack" style="flex-grow: 3"> <img src="sunspot.jpg" alt="skin with sunspots" style="width:200; height:200;">
	</div>
  <div class="makeMeStack" style="flex-grow: 2" ><img src="download.jpg" alt="before and after" style="width:200; height: 200;"></div>
  <div class="makeMeStack" style="flex-grow: 1" ><img src="skinbetter.jpg" alt="skinbetter product" style="width:200; height:200;"></div>
  <div style="flex-grow: 2" > <p>Several people have problems with age spots or sun damage due to over exposure. Thankfully there are several ways to reverse this damage. Some options are minimally invasive and lighter spots can be corrected with skincare products. </p></div>
		</div>
		
<div id="accordion">
  <h3>What to use</h3>
  <div>
    <p>
    Insert paragraph here about what products to use. 
    </p>
  </div>
  <h3>Procedures</h3>
  <div>
    <p>
   Paragraph here with procedures and descriptions.
    </p>
  </div>		
		</div>
		
		<div><footer>The End</footer></div>
	  </body>
		</html>
 

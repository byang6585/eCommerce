<doctype!>

<html>

	<head>

	

		<title> Buytel </title>

			<style>

			ul {

    list-style-type: none;

    margin: 0;

    padding: 0;

    overflow: hidden;

    background-color: blue;

}

li {

    float: left;

}

li a, .dropbtn {

    display: inline-block;

    color: white;

    text-align: center;

    padding: 14px 16px;

    text-decoration: none;

}

li a:hover, .dropdown:hover .dropbtn {

    background-color: green;

}

li.dropdown {

    display: inline-block;

}

.dropdown-content {

    display: none;

    position: absolute;

    background-color: #f9f9f9;

    min-width: 160px;

    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);

    z-index: 1;

}

.dropdown-content a {

    color: black;

    padding: 12px 16px;

    text-decoration: none;

    display: block;

    text-align: left;

}

.dropdown-content a:hover {background-color: #f1f1f1}

.dropdown:hover .dropdown-content {

    display: block;

}

			

			

			

			

			

			.dropbtn {

    background-color: #4CAF50;

    color: white;

    padding: 16px;

    font-size: 16px;

    border: none;

    cursor: pointer;

}

.dropbtn:hover, .dropbtn:focus {

    background-color: #3e8e41;

}

#myInput {

    border-box: box-sizing;

    background-image: url('searchicon.png');

    background-position: 14px 12px;

    background-repeat: no-repeat;

    font-size: 16px;

    padding: 14px 20px 12px 45px;

    border: none;

}

.dropdown {

    position: relative;

    display: inline-block;

}

.dropdown-content {

    display: none;

    position: absolute;

    background-color: #f6f6f6;

    min-width: 230px;

    overflow: auto;

    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);

    z-index: 1;

}

.dropdown-content a {

    color: black;

    padding: 12px 16px;

    text-decoration: none;

    display: block;

}

.dropdown a:hover {background-color: #ddd}

.show {display:block;}

			

			

			img {width:300px}

			input{width:100px;

			text-align:left;}

			h1 {color:red;}

			body{background-color: yellow;}

			h2 {color:blue;} 

				

				

			</style>

			<script>

			function myFunction() {

    document.getElementById("myDropdown").classList.toggle("show");

}

function filterFunction() {

    var input, filter, ul, li, a, i;

    input = document.getElementById("myInput");

    filter = input.value.toUpperCase();

    div = document.getElementById("myDropdown");

    a = div.getElementsByTagName("a");

    for (i = 0; i < a.length; i++) {

        if (a[i].innerHTML.toUpperCase().indexOf(filter) > -1) {

            a[i].style.display = "";

        } else {

            a[i].style.display = "none";

        }

    }

}

			function Money(){

			var Output = document.getElementById("Output");

			var Qty1 = document.getElementById("Qty1");

			var Qty2 = document.getElementById("Qty2");

			var Qty3 = document.getElementById("Qty3");

			var Rprice1 = document.getElementById("Rprice1");

			var Rprice2 = document.getElementById("Rprice2");

			var Rprice3 = document.getElementById("Rprice3");

			var Customer = parseFloat(Rprice1.value)*parseFloat(Qty1.value)+ parseFloat(Rprice2.value)*parseFloat(Qty2.value)+ parseFloat(Rprice3.value)*parseFloat(Qty3.value);

			var Cost = parseFloat(Wprice1.value)*parseFloat(Qty1.value)+ parseFloat(Wprice2.value)*parseFloat(Qty2.value)+ parseFloat(Wprice3.value)*parseFloat(Qty3.value);

			var tax1 = Customer*(0.0875)

			var item = parseFloat(Qty1.value)+ parseFloat(Qty2.value)+ parseFloat(Qty3.value);

			var bought = parseFloat(Rprice1.value);

			var tax2 = bought*0.0875

			var Shipping = 25

			var retail = bought + tax2 + Shipping 

			var profit = Customer - Cost;

			if (bought <= 100){

				Shipping = 25;

			}

			else if (bought >= 100 && bought < 200){

				Shipping = 10;

			}

			else if (bought >=200){

				Shipping = 0;

			}

			var info = "";

			info += "Customer"+"<hr>";

			info += "<hr> " + "<br>";

			info += "Subtotal: " + bought.toFixed(2) +"<br>";

			info += "Tax: " + tax2 +"<br>";

			info += "Shipping: " + Shipping +"<br>";

			info += "<hr> " + "<br>";

			info += "Total: " + retail.toFixed(2)+ "<br>";

			info += "<br>";

			info += "Company"+"<hr>";

			info += "<hr> " + "<br>";

			info += "Earned: " + Customer.toFixed(2) +"<br>";

			info += "Cost: " + Cost +"<br>";

			info += "<hr> " + "<br>";

			info += "Profit: " + profit.toFixed(2) + "<br>";

			

			output.innerHTML = info;

			

			}

			

			

			

			</script>

	</head>

	<body>

	<ul>

  <li><a href="#home">Buytel</a></li>

  <li><a href="#news">Home</a></li>

  <li><a href= "#">Info</a></li>

  

   <li><a href= "#">Sign up</a></li>

   <li><a href= "#">Account</a></li>

  

    </div>

  </li>

</ul><br>







	<div class="dropdown">

<button onclick="myFunction()" class="dropbtn">Search Button</button>

  <div id="myDropdown" class="dropdown-content">

    <input type="text" placeholder="Search.." id="myInput" onkeyup="filterFunction()">

    <a href="#about">About</a>

    <a href="#base">Base</a>

    <a href="#contact">Contact</a>

    <a href="#custom">Custom</a>

    <a href="#support">Support</a>

  </div>

</div>



	

	<div>

		<h1> Toyota Camery 2007</h1>

		<img src= "toyota.jpg"><br>

		<span>Price:$<input type = "text" id = "Rprice1" placeholder = "Price of car">  </span>

		<p>A reliable used car. Has gotten better over time. 10 years, hasn't changed a bit. Last deal, hurry!</p>

		<h2> 50% off until November 10,2017! Get it now!</h2>

	

		Quantity:<input type = "text" id = "Qty1"placeholder = "How many?"> <br>

		

		

		<h1> Toy Yoda</h1><br>

		<img src= "yoda.jpg"><br>

		<span>Price:$<input type = "text" id = "Rprice2" placeholder = "Price of toy"></span>

		<p>A well worthed toy that exceeds its value. Will not regret your purchase.Plus, a great way of pranking your friends of you buying them a Toyota!</p>

		

		

		Quantity:<input type = "text" id = "Qty2"placeholder = "How many?"> <br>

		

		<h1> Xbox 1</h1><br>

		<img src= "console.jpg"><br>

		<span>Price:$<input type = "text" id = "Rprice3" placeholder = "Price of console"></span>

		<p>The console still works! still is the same as when the console was made. Great Deal here, so come on and purchase it!</p>

		<h2> 15% off until January 10,2018! Get it now!</h2>

		

		Quantity:<input type = "text" id = "Qty3"placeholder = "How many?"> <br>

		

		<button onclick= "Money()"> Profit and Money</button><br>

		

		

		

		Cost of car:$<input type = "text" id = "Wprice1" placeholder = "Enter cost of Car?"><br>

		

		Cost of toy yoda:$<input type = "text" id = "Wprice2" placeholder = "Enter cost of toy Yoda?"><br>

		Cost of Console:$<input type = "text" id = "Wprice3" placeholder = "Enter cost of the Console?"><br>

		

		

		

		

		

		

		<div id = "output"></div>

	



		

		

		

		

		

		

	</div>

	

	</body>

</html>

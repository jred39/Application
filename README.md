#Appliction<!DOCTYPE html>
<html>
<head>
<style>
body {
	background-color:rgb(230,230,230);
}

h1 {
	margin-left:25%;
	text-align:center;
	color:maroon; 
 	padding:10px; 
 	margin:20px; 
 	background-color:rgb(230,230,230); 
 	font-size:40px; 
 	border: 3px solid maroon; 
 	width:500px; 
 	border-radius:4px; 
 	box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    font-family:Arial, Helvetica, sans-serif;
}
button {
	margin-left:50%;
    font-family:Arial, Helvetica, sans-serif;
}
#words {
	font-size:20px;
    font-family:Arial, Helvetica, sans-serif;
    text-align:center;
}

ul {
    list-style-type:none;
    margin:0;
    padding:0;
    width:150px;
    background-color:#f1f1f1;
    margin-left:10px;
    margin-top:10px;
}
#bottom {
	height:100px;
    color:maroon;
    margin-bottom:0%;
    background-color:#f1f1f1;
    box-shadow: 4px 0 4px 4px rgba(0, 0, 0, 0.2), 0 4px 4px 0 rgba(0, 0, 0, 0.19);
}
li a {
    display: block;
    color:maroon;
    padding: 8px 16px;
    text-decoration: none;
    font-family:Arial, Helvetica, sans-serif;
    
}


li a:hover {
    background-color: #555;
    color: white;
}
</style>

</head>
<body>
<div id="pic"></div>

<h1>Scripture Mastery App</h1>
<img src="book.jpg">
<p id="words">Click the button to get your scripture mastery verse for the day.</p>
<ul>
  <li><a href="#home">New Scripture</a></li>
  <li><a href="#news">Memorized</a></li>
  <li><a href="#contact">Read Chapter</a></li>
  <li><a href="#about">About</a></li>
</ul>
<button type="button" onclick="loadDoc()">Get Scripture</button><div id="bottom"></div>
<script>
function loadDoc() {  
var xhttp;  
	if (window.XMLHttpRequest) {    
	xhttp = new XMLHttpRequest();    
	} 
		else {    
			xhttp = new ActiveXObject("Microsoft.XMLHTTP");  
		}  
xhttp.onreadystatechange = function() {    
	if (this.readyState == 4 && this.status == 200) {      
		document.getElementById("words").innerHTML = this.responseText;    
	}  
};  
xhttp.open("GET",https://jred39.github.io/Data/, true);  
xhttp.send();}
</script>
</body>
</html>

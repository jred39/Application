<!DOCTYPE html>
<html>
<head>
<title>Application</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body {
 //background-color:rgb(230,230,230);
	background-image:url(http://hd-wall-papers.com/images/wallpapers/bible-wallpaper/bible-wallpaper-15.jpg);
}
i {
 padding:4px;
	
}
h1 {
 text-align:center;
	margin-left:30%;
 color:maroon;
  padding:10px;
  //margin:20px;
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
	margin-top:15%;
	font-family:Arial, Helvetica, sans-serif;
	
}
#words {
 font-size:20px;
	font-family:Arial, Helvetica, sans-serif;
	text-align:center;
	margin-left:30%;
	color:rgb(100,100,100);
	border:2px solid grey;
	height:40px;
	background-color:rgb(230,230,230);
	padding:5px;
	
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
	margin-top:20px;
	background-color:#f1f1f1;
}
li a {
	display: block;
	color:maroon;
	padding: 8px 16px;
	text-decoration: none;
	font-family:Arial, Helvetica, sans-serif;
	
}
i:hover {
 font-size:25px;
}
li a:hover {
	background-color: #555;
	color: white;
}
img{
 height:80px;
	width:40px;
	margin-top:30px;
	margin-left:60px;
}
</style>
<script>
function getVerse() {
 var verseNum = 2 //Math.floor((Math.random() * 2) + 2);
	var verse
	if (verseNum = 1) {
	 
    	verse = "1 Nephi 3:7 <br> I will go and do."
  //
  //document.getElementById("words").innerHTML=" 1 Nephi 3:7";
	}
	 else if (verseNum = 2) {
    	 document.getElementById("words").style.color = "red";
   verse = " 2 Nephi 2:25 <br> Adam fell.";
    	}
    	document.getElementById("words").innerHTML=verse;
    	document.getElementById("words").style.color = "blue";
}
</script>
</head>
<body>
<div id="pic"></div>
<h1>Scripture Mastery App</h1>
<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">Memorized</a></li>
  <li><a href="#contact">Read Chapter</a></li>
  <li><a href="#about">About</a></li>
</ul>
<img src="https://s-media-cache-ak0.pinimg.com/736x/f6/77/ca/f677ca9647ade446e3b0a23871bd4ee0.jpg">
<div id="words">Click the button to get your scripture mastery verse for the day.</div>
<button type="button" onclick="getVerse()">Get Scripture</button>
<i class="fa fa-book" style="font-size:20px;"></i>
<i class="fa fa-heart" style="font-size:20px;"></i>
<i class="fa fa-save" style="font-size:20px;"></i>
<i class="fa fa-file" style="font-size:20px;"></i>
<i class="fa fa-bars" style="font-size:20px;"></i>
<div id="bottom"></div>

</body>
</html>



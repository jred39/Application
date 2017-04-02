<!DOCTYPE html>
<html>
<head>
<title>Application</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body {
	background-image:url(http://hd-wall-papers.com/images/wallpapers/bible-wallpaper/bible-wallpaper-15.jpg);
    padding:1px;
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
    position:static;
    height:40px;
    border-radius:4px;
    
	
}
#words {
 font-size:20px;
	font-family:Arial, Helvetica, sans-serif;
	text-align:center;
	margin-left:50%;
    top:30%;
	color:rgb(100,100,100);
	border:2px solid grey;
	height:auto;
    position:static;
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
	color:blue;
	margin-top:20px;
	background-color:#f1f1f1;
}
li a {
	display: block;
	color:maroon;
	padding:8px 16px;
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
 var verseNum = Math.floor((Math.random() * 10) + 1);
	var verse
    var chapter
	if (verseNum == 1) {
    	verse = "1 Nephi 3:7 <br> And it came to pass that I, Nephi, said unto my father: I will go and do the things which the Lord hath commanded, for I know that the Lord giveth no commandments unto the children of men, save he shall prepare a way for them that they may accomplish the thing which he commandeth them."
        //chapter = "https://www.lds.org/scriptures/bofm/1-ne/3.7?lang=eng#6";
	}
	 else if (verseNum == 2) {
    	 document.getElementById("words").style.color = "red";
   verse = " 2 Nephi 2:25 <br> Adam fell that men might be; and men are, that they might have joy.";
    	}
     else if (verseNum == 3) {
    	 document.getElementById("words").style.color = "red";
   verse = " 2 Nephi 2:27 <br> Wherefore, men are free according to the flesh; and all things are given them which are expedient unto man. And they are free to choose liberty and eternal life, through the great Mediator of all men, or to choose captivity and death, according to the captivity and power of the devil; for he seeketh that all men might be miserable like unto himself.";
    	}
    	document.getElementById("words").innerHTML = verse;
        document.getElementById("next").innerHTML = "<strong>New Scripture";
    	document.getElementById("words").style.color = "blue";
        document.getElementById("read").innerHTML = "Read Chapter";
        document.getElementById("read").href = "https://www.lds.org/scriptures/bofm/1-ne/3.7?lang=eng#6";
}
</script>
</head>
<body>

<h1>Scripture Mastery App</h1>

<ul>
  <li><a href="#home"><strong>Home</a></li>
  <li><a href="#news">Memorized</a></li>
  <li><a href="https://www.lds.org/manual/book-of-mormon-seminary-teacher-manual-2013/appendix/introduction-to-scripture-mastery?lang=eng">lds.org</a></li>
  <li><a href="#about">About</strong></a></li>
</ul>

<img src="https://s-media-cache-ak0.pinimg.com/736x/f6/77/ca/f677ca9647ade446e3b0a23871bd4ee0.jpg">

<div id="words">Click the button to get a Book of Mormon scripture mastery verse.</div>

<button id="read" href="#"></button>

<button id="next" type="button" onclick="getVerse()"><strong>Get Scripture</button>

<div id="bottom">
<i class="fa fa-book" style="font-size:20px;"></i>
<i class="fa fa-heart" style="font-size:20px;"></i>
<i class="fa fa-save" style="font-size:20px;"></i>
<i class="fa fa-file" style="font-size:20px;"></i>
<i class="fa fa-bars" style="font-size:20px;"></i>

</div>

</body>
</html>



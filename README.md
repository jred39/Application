# Application<!DOCTYPE html>
<html>
<body>
<h1>Scripture Verse App</h1>
<p id="demo">Click the button to get a random scripture for the day.</p>
<button type="button" onclick="loadDoc()">Change Content</button>
<script>function loadDoc() {  
var xhttp;  
if (window.XMLHttpRequest) {    
xhttp = new XMLHttpRequest();    
} 
else {    
xhttp = new ActiveXObject("Microsoft.XMLHTTP");  
}  
xhttp.onreadystatechange = function() {    
if (this.readyState == 4 && this.status == 200) {      
document.getElementById("demo").innerHTML = this.responseText;    
}  
};  
xhttp.open("GET",https://jred39.github.io/Data/, true);  
xhttp.send();}
</script>
</body>
</html>

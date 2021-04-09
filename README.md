<!DOCTYPE html>
<html>
<head><title>Q4 website pog</title></head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial;
  margin: 0px;
}

/* Style the tab */
.tab {
  overflow: hidden;
  border: 0px solid #ccc;
  background-color: black;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
}

/* Style the buttons inside the tab */
.tab button {
  background-color: inherit;
  float: right;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
  color: white;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ceb18d;
}

.tabcontent {
  display: none;
  padding: 50px 145px;
  width: 850px;
  margin: 80px 107px;
}

.col {
  background-color: #ceb18d;
  padding: 0px;
  color: white;
  margin: 100px 100px;
}

.con {
  background-color: white;
  margin: 50px 70px 0px 750px;
}

</style>
</head>
<body bgcolor="#ceb18d">

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'Menu')">Menu</button>
  <button class="tablinks" onclick="openCity(event, 'Home')" id="defaultOpen">Home</button>
</div>

<div class="con">
 <div id="Menu" class="tabcontent">
  <h3>MENU:</h3>
  <p><h3>Appetizers:<br />
     <br />
     Matcha Pancake<br />
     waffles<br />
     Prawn Dumplings<br />
     Siopao<br />
     Siomai<br />
     <br />
     Rice meals:<br />
     <br />
     Adobo<br />
     Tapsilog<br />
     <br />
     Soup:<br />
     <br />
     Congee<br />
     Corn Soup<br />
     Ramen<br />
     <br />
     Drinks:<br />
     <br />
     Matcha Milktea<br />
     Ice tea<br />
     Frappe<br />
     Coffee:<br />
     Vanilla<br />
     Mocha<br />
     Cuppacino<br />
     Iced<br />
     <br />
     Deserts:<br />
     <br />
     Mochi Balls<br />
     Halo-Halo<br />
     </p></h3>
 </div>
</div>

<div class="col">
 <div id="Home" class="tabcontent">
  <h1>Welcome to our Cafe<br />
  <p><i>We've got drinks and, <br />We've got food</i></h1>
 </div>
</div>

<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
   
</body>
</html> 

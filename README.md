<!DOCTYPE>
<html lang="en">
  <head>
    <link rel="stylesheet" href="styles.css">
   <meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Personal Profile</title>
  </head>


  

  <nav id="navbar" class="nav">
    <div class="logo">
      <img href="index.html" src="logo.png" alt="Yellow logo with a bounce house in the center.">
    </div>
    
    <ul class="nav-list">
      <li>
        <a  id="home" href="index.html">HOME</a>
      </li>
      <li>
        <a id="bounce" href="bounce_house.html">BOUNCE HOUSE</a>
      </li>
      <li>
        <a id="balloons" href="balloons.html">BALLOONS</a>
      </li>
      <li>
        <a id="chairs" href="#projects">CHAIRS</a>
      </li>
      <li>
        <a id="tables" href="#projects">TABLES</a>
      </li>
      <li>
        <a id="about" href="about.html">ABOUT</a>
      </li>
      <li>
        <a id="contact" href="contact_us.html">CONTACT</a>
      </li>
    </ul>
  </nav>


  <section id="slideshow-container" class="slideshow-container">
    <div class="centered">Pick us to celebrate with you!
    </div>

    <div class="mySlides fade">
      <img src="medium-shot-girl-holding-stick.jpg">
      </div>
    <div class="mySlides fade">
      <img src="full-shot-smiley-girl-bounce-house.jpg">
      </div>
    <div class="mySlides fade">
      <img src="main_img.jpg">
      </div>
    <div class="mySlides fade">
      <img src="portrait-young-girls-party-with-balloons.jpg">
      </div>

  </section>

  <section class="picSec">
  <div class="sec1">
    <div class="events right"><h1>Birthdays!</h1></div>
    <img  src="ezgif.com-crop.jpg" alt="Red tinted image of a camera set up.">
  </div>
  <div class="sec2">
    <div class="events left"><h1>Graduation!</h1></div>
    <img  src="grad_balloons.jpg" alt="Red tinted image of a camera set up.">
  </div>
  </section>



  <footer >
    <p class="footer"><span>OPENING HOURS:<br />
      Monday-Friday: 8am-8pm<br />Saturday-Sunday: 8am-4pm
    </span ></p>
    <p class="footer">
    <address>
    Jenny's Party Rentals & Gifts<br />
    1027 Long Beach Blvd, <br />
    Lynwood, CA 90262<br />
    </address>
    </p>
    <p>Image by <a href="https://www.freepik.com/free-photo/full-shot-smiley-girl-bounce-house_29801462.htm#query=bounce%20house&position=0&from_view=search&track=ais">Freepik</a></p>
  </footer>
  </body>
  


<style>
  .centered li{
      list-style-type: none;
      font-size: 4.5vw;
    }

.picSec{
  padding: 5vw 7vw;
}
.picSec img{
  width: 45%;
  height: auto;
  margin-top: 10vw;
  margin-left:5vw;
  border-radius: 3vw;

}

.events{
  margin: 20vw 1vw;
  font-size: 3vw;
}

.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 98;
  color:white;
  font-size: 6vw;
  text-align: center;
  color: #fff;
    text-shadow: 1px 0 0 #000, 0 -1px 0 #000, 0 1px 0 #000, -1px 0 0 #000;
  font-weight: 700;
}


html {
    scroll-behavior: smooth;
}
*{
    box-sizing: inherit;
    margin: 0;
    padding:0;
    
}
  
.left{
  float:left;
  margin-left: 5vw;

}
.right{
  float: right;
  margin-right: 5vw;

}
.logo img{
  width: 5vw;
  margin: .5vw 1.5vw;
  z-index: 100;

}
.nav {
  display: flex;
  justify-content:left;
  position: fixed;
  top: 0;
  width: 100%;
  background: linear-gradient(rgb(0,0,0,1), rgb(0,0,0,0));
  z-index: 100;
}

nav li {
  display:inline-block;
  list-style: none;
}

nav a {
  text-decoration: none;
  color:white;
  padding: 2.5vw;
  font-size: 1vw;
  display: block;
}

footer{
  margin-top:10vw;
  display: flex;
  background-color: #ead1dc;
  max-width: 100%;
  padding: 10px 40px;
  justify-content: space-around;
  }
@media (hover: hover) {
  #home:hover {
    color: white;
    background: red;
  }
  #bounce:hover {
    color: white;
    background: blue;
  }
  #balloons:hover {
    color: white;
    background: purple;
  }
  #chairs:hover {
    color: white;
    background: orange;
  }
  #tables:hover {
    color: white;
    background: green;
  }
  #about:hover {
    color: white;
    background: indigo;
  }
  #contact:hover {
    color: white;
    background: violet;
  }
  }

.slideshow-container {
  position: relative;
  width:100%;
  height;auto:
 }

.mySlides img{
  width:100%;
  object-fit: cover;
  max-width: 100%;
  height: auto;
  margin:0;
  opacity:1;
}

.fade {
  animation-name:fade;
  animation-duration:3s;
  
}

@keyframes fade {
  from {opacity: .8} 
  to {opacity: 1}
}

    
</style>

<script>
  let slideIndex = 0;
  showSlides();

  function showSlides() {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {
    slideIndex = 1
    }    
  
  slides[slideIndex-1].style.display = "block";  
  setTimeout(showSlides, 7000); 
}
</script>
</html>

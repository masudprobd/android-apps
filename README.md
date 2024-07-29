



<style>

@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,900;1,700&display=swap");

/* variables */
:root{
  --font-family: 'Roboto',sans-serif;
  --normal-font: 400;
  --bold-font: 700;
  --bolder-font: 900;
  --bg-color: #fcfcfc;
  --primary-color: #250C77;
  --secondary-color: #ED642B;
  --primary-shadow: #8b8eaf;
  --secondary-shadow: #a17a69;
  --bottom-margin: 0.5rem;
  --bottom-margin-2: 1rem;
  --line-height: 1.7rem;
  --transition: 0.3s;
}
/* variables end */

html{
  scroll-behaviour: smooth;
}

/* css reset  */
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul{
  list-style-type: none;
}
a{
  text-decoration: none;
  color: var(--bg-color);
}
a:hover{
  cursor: pointer;
  color: var(--secondary-color);
}

body{
  font-family: var(--font-family);
}

/* navigation */
nav{
  position: sticky;
  top: 0;
  left: 0;
  z-index: 1;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: var(--primary-color); 
  padding: 1.5rem 3.5rem;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.5);
}
nav h1{
  color: var(--bg-color);
}
nav h1 sup{
  color: var(--secondary-color);
}
nav a{
  color: var(--bg-color);
  transition: var(--transition);
}
nav a:hover{
  color: var(--secondary-color);
  border-bottom: 2px solid var(--secondary-color);
}

nav ul{
  display: flex;
  gap: 1.9rem;
}
nav ul li{
  font-weight: var(--bold-font);
}

.burger-menu{
  color: var(--bg-color);
  background: transparent;
  border: 0;
  font-size: 2rem;
  cursor: pointer;
  display: none;
}
/* navigation end */

/* hero section */

.hero-section-slider{
  height: 100vh;
  background-size: cover;
  background-image: url(https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8Z2FtaW5nfGVufDB8fDB8fA%3D%3D&w=1000&q=80);
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  animation: slider 4s ease-in infinite;
}
.hero-section-slider h2{
  color: var(--bg-color);
  border-bottom: 2.5px solid var(--secondary-color);
  text-shadow: 0 3px 2px var(--secondary-color);
  text-align: center;
  font-size: 2.5rem;
  font-weight: var(--bolder-font);
}
/* ------------------ */
/* about section */
.about{
  background-color: var(--bg-color);
  padding: 1rem 6rem;
}
.about h2{
  text-align: center;
  margin-bottom: var(--bottom-margin-2);
}
.about p{
  color: dodgerblue;
  line-height: var(--line-height);
  padding: 0.4rem;
}
/* ---------------------- */
/* services */
.services{
  background-color: var(--bg-color);
  padding: 32px 0;
  margin-top: 2rem;
}
.services-header{
  text-align: center;
  font-weight: var(--bolder-font);
  margin-bottom: var(--bottom-margin-2);
}
.services-wraper{
  padding: 1rem 1rem;
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.service-container{
  flex: 1 1 18.750rem;
  width: 21.875rem;
  padding: 1rem;
  box-shadow: 0 3px 5px var(--secondary-shadow);
}
.service-pic{
  width: 65%;
  height: 60%;
  box-shadow: 0 0 5px var(--primary-color);
  
}
.service-container:nth-child(2) .service-pic{
  width: 50%;
}
.service-title{
  font-weight: var(--bold-font);
  margin-bottom: var(--bottom-margin);
  border-bottom: 2px solid var(--secondary-color);
}
.service-btn{
  color: dodgerblue;
  font-weight: var(--bold-font);
  transition: var(--transition);
}
.service-btn:hover{
  border-bottom: 2px solid var(--secondary-color);
}
/* ------------- */
/* footer */
footer{
  background-color: var(--primary-color);
  padding: 2.5rem;
  margin: 2rem 0 0;
  
}
.first-part{
  color: var(--primary-shadow);
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  text-align: center;
  gap: 2rem;
  margin-bottom: var(--bottom-margin-2);
  border-bottom: 2px solid var(--secondary-color);
}
.first-part h1{
  color: var(--bg-color);
}
.first-part h1 sup{
  color: var(--secondary-color);
}
.second-part{
  margin-top: 0.875rem;
  font-size: 1.2rem;
  color: var(--bg-color);
  text-align: center;
  
}
.second-part span{
  font-size: 1.5rem;
  color: aqua;
}

/*  ----------------------------------------------------------   */
/* slider animation images */
@keyframes slider{
  10%{background-image: url(https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8Z2FtaW5nfGVufDB8fDB8fA%3D%3D&w=1000&q=80);}
  30%{background-image: url(https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=871&q=80);}
  50%{background-image: url(https://images.unsplash.com/photo-1538481199705-c710c4e965fc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=965&q=80);}
  70%{background-image: url(https://images.unsplash.com/photo-1616588589676-62b3bd4ff6d2?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1032&q=80);}
  90%{background-image: url(https://images.unsplash.com/photo-1495954222046-2c427ecb546d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1032&q=80);}
  100%{background-image: url(https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8Z2FtaW5nfGVufDB8fDB8fA%3D%3D&w=1000&q=80);}
}
/* ------------------------------------------------------------- */

/* responsive */
@media screen and (max-width: 720px){
/*  navigation  */
  nav{
    padding: 1.5rem 1rem;
  }
  nav ul{
    position: fixed;
    background-color: rgba(0,0,0,0.5);
    flex-direction: column;
    top: 86px;
    left: 10%;
    width: 80%;
    text-align: center;
    transform: translateX(120%);
    transition: transform 0.5s ease-in;
  }
  nav ul li{
    margin: 8px;
  }
  nav ul li a{
    color: aqua;
  }
  .burger-menu{
    display: block;
  }
/*   for showing our menu  we toggle this class to nav*/
  nav ul.show{
    transform: translateX(0);
  }
  
/*  hero section heading  */
  .hero-section h2{
    font-size: 2rem;
    border-bottom: none;
  }
}

@media screen and (max-width: 440px){
/*   footer */
  .first-part{
    flex-direction: column;
  }
}
  </style>





<!-- navigation menu -->
<nav>
  <h1>GAME | <sup>over</sup></h1>
  <ul class="navigation">
    <li><a class="nav-link" href="#home">Home</a></li>
    <li><a class="nav-link" href="#about">About</a></li>
    <li><a class="nav-link" href="#services">Services</a></li>
    <li><a class="nav-link" href="#blog">Blog</a></li>
    <li><a class="nav-link" href="#features">Features</a></li>
    <li><a class="nav-link" href="#contact">Contact</a></li>
  </ul>
  
  <button class="burger-menu" id="burger-menu">&#9776;</button>
  
</nav>
<!-- ----------------------- -->
<!-- hero section -->
<section class="hero-section" id="home">
  <div class="hero-section-slider">
    <h2>Welcome 2 The Gaming World</h2>
  </div>
</section>
<!-- ------------------------ -->
<!-- about section -->
<section class="about" id="about">
  <h2>About our Gaming World</h2>
  <p>
    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sint eaque accusamus aperiam quisquam libero ad, ab eos cumque nobis magnam deleniti et, facilis molestiae numquam exercitationem beatae tempora quae quas, laboriosam provident minima sapiente sit. Tempore fuga ea necessitatibus nisi ipsum quas molestiae ad excepturi error quaerat dolorem perspiciatis animi similique autem, neque doloribus eos a rem repudiandae id aspernatur incidunt quibusdam assumenda magnam? Aliquam vitae, alias rem consequatur, sed corrupti pariatur voluptas dolores eaque porro labore atque officia rerum consectetur repellat corporis recusandae, tenetur iure aperiam dicta maiores fuga fugit dolore facere. Pariatur, inventore! Tempore, dolores corporis. Delectus, optio?
  </p>
  <p>
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quas, quam. Voluptate facilis nulla quaerat necessitatibus deserunt eius quia quisquam tempora!
  </p>
  
</section>
<!-- ---------------------- -->
<!-- services -->
<section class="services" id="services">
  <h2 class="services-header">Our Top Services</h2>
  <div class="services-wraper">
    <div class="service-container">
      <img 
           src="https://cloudgame.press/wp-content/uploads/2020/08/cloud-gaming-kak-rabotaet-1280x720.jpg" 
           alt="cloud-services"
           loading="lazy"
           class="service-pic"
       />
      <h3 class="service-title">Cloud Services</h3>
      <p class="service-detail">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet nobis quia similique sapiente consectetur sit cupiditate tempora eos laboriosam voluptates.
      </p>
      <a href="#" class="service-btn">Buy Now</a>
    </div>
    <div class="service-container">
      <img 
           src="https://i.ytimg.com/vi/n3Qxo79HoZk/hqdefault.jpg" 
           alt="unity-gaming-services"
           loading="lazy"
           class="service-pic"
       />
      <h3 class="service-title">Unity Gaming</h3>
      <p class="service-detail">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet nobis quia similique sapiente consectetur sit cupiditate tempora eos laboriosam voluptates.
      </p>
      <a href="#" class="service-btn">Buy Now</a>
    </div>
    <div class="service-container">
      <img 
           src="https://sw.cool3c.com/user/104471/2021/09b54019-4e3f-4fe7-8474-71029981f431.jpg?fit=max&w=2400&q=80" 
           alt="xbox-services"
           loading="lazy"
           class="service-pic"
       />
      <h3 class="service-title">X-Box Subscription</h3>
      <p class="service-detail">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet nobis quia similique sapiente consectetur sit cupiditate tempora eos laboriosam voluptates.
      </p>
      <a href="#" class="service-btn">Buy Now</a>
    </div>
  </div>
</section>
<!-- footer -->
<footer>
  <div class="first-part">
    <div class="useful-links">
      <h3>Useful Links</h3>
      <ul>
        <li><a href="#">Our Products</a></li>
        <li><a href="#">Discount Offers</a></li>
        <li><a href="#">Gaming Tools</a></li>
      </ul>
    </div>
    <h1>GAME | <sup>over</sup></h1>
    <div class="contact" id="contact">
      <h2>Contact-us</h2>
      <ul>
        <li><a href="#">Facebook</a></li>
        <li><a href="#">Instagram</a></li>
        <li><a href="#">G-mail</a></li>
        <li><a href="#">Linkedin</a></li>
      </ul>
    </div>
  
  </div>
  <div class="second-part">
    <p class="copy">&copy; Copyright 2024</p>
    <p class="copy">
      built with <span>&#x2661;</span> by <a href="#">masudprobd</a>
    </p>
  </div>
</footer>


<script>
// nav hamburger-menu selection
const menubtn = document.querySelector('#burger-menu');
const ul = document.querySelector('nav ul');
const nav = document.querySelector('nav');

menubtn.addEventListener('click', () => {
  ul.classList.toggle('show');
});

// click hamburger menu when link is clicked
var navlinks = document.querySelectorAll('.nav-link');
navlinks.forEach((link) => 
             link.addEventListener('click', ()=> {
                ul.classList.remove('show');  
  })
);</script>

<template   >
    <section class="head">
        <div class="container flex1">
          <div class="scoial">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-youtube"></i>
          </div>
          <div class="logo">
            <img src="../../../public/theme1/image/logo1.png" alt="">
          </div>
          <div class="address">
            <i class="fas fa-map-marker-alt"></i>
            <span>7, Hyoryeong-ro 51-gil, Seocho-gu, Seoul, Republic of Korea</span>
          </div>
        </div>
      </section>
    
    
      <header class="header">
        <div class="container">
          <nav class="navbar flex1">
            <div class="sticky_logo logo">
              <img src="../../../public/theme1/image/logo1.png" alt=""> 
            </div>
    
            <ul class="nav-menu">
              <li> <a href="#home">Home</a> </li>
              <li> <a href="#about">about</a> </li>
              <li> <a href="#room">room</a> </li>
              <li> <a href="#services">services</a> </li>
              <li> <a href="#shop">shop</a> </li>
              <li> <a href="#testimonials">testimonials</a> </li>
              <li> <a href="#gallary">gallary</a> </li>
              <li> <a href="#blog">blog</a> </li>
              <li> <a href="#contact">contact</a> </li>
            </ul>
            <div class="hamburger">
              <span class="bar"></span>
              <span class="bar"></span>
              <span class="bar"></span>
            </div>
    
            <div class="head_contact">
              <i class="fas fa-phone-volume"></i>
              <span>82)02-587-8990</span>
            </div>
          </nav>
        </div>
      </header>
</template>

<script>
export default {
  //name: 'Header_step',
}
/*
const hamburger = document.querySelector(".hamburger");
const navMenu = document.querySelector(".nav-menu");

hamburger.addEventListener("click", mobliemmenu);

function mobliemmenu() {
  hamburger.classList.toggle("active");
  navMenu.classList.toggle("active");
}

    window.addEventListener("scroll", function() {
      var header = document.querySelector("header");
      header.classList.toggle("sticky", window.scrollY > 0)
    })*/
</script>
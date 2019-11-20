<template>
<div>
<div class="page">
      <div class="space">
          <p><strong>Welcome To Our Webpage</strong></p>
        <div class="contact">
          <p class="button">
            <a href="#">
                <router-link to="/login">Please Login</router-link>
                </a>
              </p>
           </div>
        </div>
      <p class="intro"> There are tons of designs that I will soon incorperate into my website. It is a beautiful work in progress. This small start will hopefully become a fully functioning website in the future.</p>
    </div>
    <router-view></router-view>
</div>
</template>

<style>
/* Background and Body */

body {
  background-image: url("https://s15.postimg.org/yfhctycij/photo_1469547371150_47620ed0c5ea.jpg");
  background-size: cover;
  position: relative;
  background-repeat: repeat-y;
}

/* main */

.blueberries {
 background-image: url("https://s15.postimg.org/yfhctycij/photo_1469547371150_47620ed0c5ea.jpg");
  margin: -8px;
  height: 680px;
  background-size: cover;
}
.color {
  background-image: url("https://s16.postimg.org/72lwqwuxh/Screen_Shot_2016_12_01_at_9_38_58_AM.png");
  background-size: cover;
  margin: -8px;
  height: 750px;
}
.buildings {
  background-image: url("https://s18.postimg.org/7socx7mjd/Screen_Shot_2016_12_05_at_1_42_11_PM.png");
  background-size: cover;
  margin: -8px;
  height: 750px;
}

/* Welcome Section */

header {
  border-bottom: 5px solid;
  margin-top: 8px;
  background-color: #DBD56E;
  padding-bottom: 5px;
}
.space {
  border: 1px solid white;
  margin: 60px;
  padding: 20px;
  text-align: center;
  font-size: 50px;
  color: #DBD56E;
}
.contact {
  margin-left: 45%;
}
.contact a:active {
  position: relative;
  bottom: -2px;
}
.button {
  font-size: 18px;
  border: 1px solid white;
  border-radius: 5px;
  width: 120px;
  background-color: grey;
  padding: 5px;
  margin-bottom: 15px;
}
.button a {
  text-decoration: none;
  color: #DBD56E;
}
.intro {
  color: white;
  font-size: 20px;
  margin: 40px;
  text-align: center;
  height: 100px;
}

/* Dropdown */

.menu2 {
  display: inline;
  font-size: 18px;
}
.menu2 li {
  display: inline;
  padding-right: 30px;
  color: black;
}
.menu2 a {
  text-decoration: none;
  color: black;
}
.menu2 a:active {
  text-decoration: none;
}
.dropdown {
  position: relative;
  display: inline-block;
  text-decoration: none;
}
.dropdown-toggle2:hover {
  /* background-color #3e8e41; */
  background-color: #4CAF50;
}
.dropdown-toggle2 {
  background-color: #DBD56E;
  padding: 7px;
  border: none;
  cursor: pointer;
}
.dropdown-menu2 {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 135px;
  overflow: auto;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  font-size: 18px;
  margin: 7px;
  margin-left: 40px;
  padding-left: 0px;
}
.dropdown-menu2 li {
  float: left;
}
.dropdown-menu2 a {
  color: black;
  padding: 12px 18px;
  text-decoration: none;
  display: block;
}
.dropdown-menu2 a:hover {
  background-color: #f1f1f1;
}

/* Next Section */

.color-info {
  padding: 5px;
  text-align: center;
}
.color-text {
  color: #9A4C95;
  font-size: 50px;
}

/* News Page */

.buildings-text {
  padding: 1px;
}
.Page2 {
  color: #C98686;
  text-align: center;
  font-size: 45px;
  font-family: Verdana;
  text-shadow: 3px 3px black;
}

/* Slideshow */

.slider {
  position: relative;
  width: 100%;
  height: 470px;
  border-bottom: 1px solid #ddd;
}
.slide {
  background: transparent url('https://s3.amazonaws.com/codecademy-content/courses/ltp2/img/flipboard/feature-gradient-transparent.png') center center no-repeat;
  background-size: cover;
  display: none;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.active-slide {
    display: block;
}

.slide-copy h1 {
  color: #363636;
  font-family: 'Oswald', sans-serif;
  font-weight: 400;
  font-size: 40px;
  margin-top: 60px;
  margin-bottom: 0px;
}
.slide-copy h2 {
  color: #b7b7b7;
  font-family: 'Oswald', sans-serif;
  font-weight: 400;
  font-size: 40px;
  margin: 5px;
}
.slide-copy p {
  color: #959595;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.15em;
  line-height: 1.75em;
  margin-bottom: 15px;
  margin-top: 20px;
}

.slide-img {
  text-align: right;
}

/* Slide feature */

.slide-feature {
  text-align: center;
  background-image: url('https://s24.postimg.org/6at7hp2ut/210.jpg');
  height: 470px;
}

.slide-feature img {
  margin-top: 112px;
  margin-bottom: 28px;
}

.slide-feature a {
  display: block;
  color: #6fc5e0;
  font-family: "HelveticaNeueMdCn", Helvetica, sans-serif;
  font-family: 'Oswald', sans-serif;
  font-weight: 400;
  font-size: 20px;
}

.slider-nav {
  text-align: center;
  margin-top: 20px;
}

.arrow-prev {
  margin-right: 45px;
  display: inline-block;
  vertical-align: top;
  margin-top: 9px;
}

.arrow-next {
  margin-left: 45px;
  display: inline-block;
  vertical-align: top;
  margin-top: 9px;
}

.slider-dots {
  list-style: none;
  display: inline-block;
  padding-left: 0;
  margin-bottom: 0;
}

.slider-dots li {
  color: #bbbcbc;
  display: inline;
  font-size: 30px;
  margin-right: 5px;
}

.slider-dots li.active-dot {
  color: #363636;
}

/* App links */

.get-app {
  list-style: none;
  padding-bottom: 9px;
  padding-left: 0px;
  padding-top: 9px;
}

.get-app li {
  float: left;
  margin-bottom: 5px;
  margin-right: 5px;
}

.get-app img {
  height: 50px;
}

/* Copyright */
</style>

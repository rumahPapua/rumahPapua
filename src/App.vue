<template>
  <div id="app">
    <div id="nav">
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">
          <router-link to="/">Rumah Papua</router-link>
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item">
              <a class="nav-link" href="#">
                <router-link to="/profile">Account</router-link>
              </a>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >About</a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">
                  <router-link to="/about">Vision & Mission</router-link>
                </a>
                <a class="dropdown-item" href="#">Insight</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Background</a>
              </div>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <router-link to="/login">Login</router-link>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <router-link to="/dashboard">Dashboard</router-link>
              </a>
            </li>
            <!-- <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
              Launch demo modal
            </button>-->
          </ul>
          <form class="form-inline my-2 my-lg-0">
            <input
              class="form-control mr-sm-2"
              type="search"
              placeholder="Search"
              aria-label="Search"
            />
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
          </form>
        </div>
      </nav>
    </div>
    <router-view />

    <div class="appFooter">
      <footer class="new_footer_area bg_color">
        <div class="new_footer_top">
          <div class="container">
            <div class="row">
              <div class="col-lg-3 col-md-6">
                <div
                  class="f_widget company_widget wow fadeInLeft"
                  data-wow-delay="0.2s"
                  style="visibility: visible; animation-delay: 0.2s; animation-name: fadeInLeft;"
                >
                  <h3 class="f-title f_600 t_color f_size_18">Get in Touch</h3>
                  <p>Don’t miss any updates of our new templates and extensions.!</p>
                  <form
                    action="#"
                    class="f_subscribe_two mailchimp"
                    method="post"
                    novalidate="true"
                    _lpchecked="1"
                  >
                    <input type="text" name="EMAIL" class="form-control memail" placeholder="Email" />
                    <button class="btn btn_get btn_get_two" type="submit">Subscribe</button>
                    <p class="mchimp-errmessage" style="display: none;"></p>
                    <p class="mchimp-sucmessage" style="display: none;"></p>
                  </form>
                </div>
              </div>
              <div class="col-lg-3 col-md-6">
                <div
                  class="f_widget about-widget pl_70 wow fadeInLeft"
                  data-wow-delay="0.4s"
                  style="visibility: visible; animation-delay: 0.4s; animation-name: fadeInLeft;"
                >
                  <h3 class="f-title f_600 t_color f_size_18">Download</h3>
                  <ul class="list-unstyled f_list">
                    <li>
                      <a href="#">Company</a>
                    </li>
                    <li>
                      <a href="#">Android App</a>
                    </li>
                    <li>
                      <a href="#">ios App</a>
                    </li>
                    <li>
                      <a href="#">Desktop</a>
                    </li>
                    <li>
                      <a href="#">Projects</a>
                    </li>
                    <li>
                      <a href="#">My tasks</a>
                    </li>
                  </ul>
                </div>
              </div>
              <div class="col-lg-3 col-md-6">
                <div
                  class="f_widget about-widget pl_70 wow fadeInLeft"
                  data-wow-delay="0.6s"
                  style="visibility: visible; animation-delay: 0.6s; animation-name: fadeInLeft;"
                >
                  <h3 class="f-title f_600 t_color f_size_18">Help</h3>
                  <ul class="list-unstyled f_list">
                    <li>
                      <a href="#">FAQ</a>
                    </li>
                    <li>
                      <a href="#">Term &amp; conditions</a>
                    </li>
                    <li>
                      <a href="#">Reporting</a>
                    </li>
                    <li>
                      <a href="#">Documentation</a>
                    </li>
                    <li>
                      <a href="#">Support Policy</a>
                    </li>
                    <li>
                      <a href="#">Privacy</a>
                    </li>
                  </ul>
                </div>
              </div>
              <div class="col-lg-3 col-md-6">
                <div
                  class="f_widget social-widget pl_70 wow fadeInLeft"
                  data-wow-delay="0.8s"
                  style="visibility: visible; animation-delay: 0.8s; animation-name: fadeInLeft;"
                >
                  <h3 class="f-title f_600 t_color f_size_18">Team Solutions</h3>
                  <div class="f_social_icon">
                    <a href="#" class="fab fa-facebook"></a>
                    <a href="#" class="fab fa-twitter"></a>
                    <a href="#" class="fab fa-linkedin"></a>
                    <a href="#" class="fab fa-pinterest"></a>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="footer_bg">
            <div class="footer_bg_one"></div>
            <div class="footer_bg_two"></div>
          </div>
        </div>
        <div class="footer_bottom">
          <!-- <div class="container">
            <div class="row align-items-center">
              <div class="col-lg-6 col-sm-7">
                <p class="mb-0 f_400">© cakecounter Inc.. 2019 All rights reserved.</p>
              </div>
              <div class="col-lg-6 col-sm-5 text-right">
                <p>
                  Made with
                  <i class="icon_heart"></i> in
                  <a href="#">CakeCounter</a>
                </p>
              </div>
            </div>
          </div> -->
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
// import AppFooter from '@/components/Footer.vue'

export default {
  components: {
    // AppFooter
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

  body {
    background: #fbfbfd;
}

.new_footer_area {
    background: #fbfbfd;
}

.new_footer_top {
    padding: 120px 0px 270px;
    position: relative;
      overflow-x: hidden;
}
.new_footer_area .footer_bottom {
    padding-top: 5px;
    padding-bottom: 50px;
}
.footer_bottom {
    font-size: 14px;
    font-weight: 300;
    line-height: 20px;
    color: #7f88a6;
    padding: 27px 0px;
}
.new_footer_top .company_widget p {
    font-size: 16px;
    font-weight: 300;
    line-height: 28px;
    color: #6a7695;
    margin-bottom: 20px;
}
.new_footer_top .company_widget .f_subscribe_two .btn_get {
    border-width: 1px;
    margin-top: 20px;
}
.btn_get_two:hover {
    background: transparent;
    color: #5e2ced;
}
.btn_get:hover {
    color: #fff;
    background: #6754e2;
    border-color: #6754e2;
    -webkit-box-shadow: none;
    box-shadow: none;
}
a:hover, a:focus, .btn:hover, .btn:focus, button:hover, button:focus {
    text-decoration: none;
    outline: none;
}

.new_footer_top .f_widget.about-widget .f_list li a:hover {
    color: #5e2ced;
}
.new_footer_top .f_widget.about-widget .f_list li {
    margin-bottom: 11px;
}
.f_widget.about-widget .f_list li:last-child {
    margin-bottom: 0px;
}
.f_widget.about-widget .f_list li {
    margin-bottom: 15px;
}
.f_widget.about-widget .f_list {
    margin-bottom: 0px;
}
.new_footer_top .f_social_icon a {
    width: 44px;
    height: 44px;
    line-height: 43px;
    background: transparent;
    border: 1px solid #e2e2eb;
    font-size: 24px;
}
.f_social_icon a {
    width: 46px;
    height: 46px;
    border-radius: 50%;
    font-size: 14px;
    line-height: 45px;
    color: #858da8;
    display: inline-block;
    background: #ebeef5;
    text-align: center;
    -webkit-transition: all 0.2s linear;
    -o-transition: all 0.2s linear;
    transition: all 0.2s linear;
}
.ti-facebook:before {
    content: "\e741";
}
.ti-twitter-alt:before {
    content: "\e74b";
}
.ti-vimeo-alt:before {
    content: "\e74a";
}
.ti-pinterest:before {
    content: "\e731";
}

.btn_get_two {
    -webkit-box-shadow: none;
    box-shadow: none;
    background: #5e2ced;
    border-color: #5e2ced;
    color: #fff;
}

.btn_get_two:hover {
    background: transparent;
    color: #5e2ced;
}

.new_footer_top .f_social_icon a:hover {
    background: #5e2ced;
    border-color: #5e2ced;
  color:white;
}
.new_footer_top .f_social_icon a + a {
    margin-left: 4px;
}
.new_footer_top .f-title {
    margin-bottom: 30px;
    color: #263b5e;
}
.f_600 {
    font-weight: 600;
}
.f_size_18 {
    font-size: 18px;
}
h1, h2, h3, h4, h5, h6 {
    color: #4b505e;
}
.new_footer_top .f_widget.about-widget .f_list li a {
    color: #6a7695;
}

.new_footer_top .footer_bg {
    position: absolute;
    bottom: 0;
    background: url("http://droitthemes.com/html/saasland/img/seo/footer_bg.png") no-repeat scroll center 0;
    width: 100%;
    height: 266px;
}

.new_footer_top .footer_bg .footer_bg_one {
    background: url("https://1.bp.blogspot.com/-mvKUJFGEc-k/XclCOUSvCnI/AAAAAAAAUAE/jnBSf6Fe5_8tjjlKrunLBXwceSNvPcp3wCLcBGAsYHQ/s1600/volks.gif") no-repeat center center;
    width: 330px;
    height: 105px;
  background-size:100%;
    position: absolute;
    bottom: 0;
    left: 30%;
    -webkit-animation: myfirst 22s linear infinite;
    animation: myfirst 22s linear infinite;
}

.new_footer_top .footer_bg .footer_bg_two {
    background: url("https://1.bp.blogspot.com/-hjgfxUW1o1g/Xck--XOdlxI/AAAAAAAAT_4/JWYFJl83usgRFMvRfoKkSDGd--_Sv04UQCLcBGAsYHQ/s1600/cyclist.gif") no-repeat center center;
    width: 88px;
    height: 100px;
  background-size:100%;
    bottom: 0;
    left: 38%;
    position: absolute;
    -webkit-animation: myfirst 30s linear infinite;
    animation: myfirst 30s linear infinite;
}

@-moz-keyframes myfirst {
  0% {
    left: -25%;
  }
  100% {
    left: 100%;
  }
}

@-webkit-keyframes myfirst {
  0% {
    left: -25%;
  }
  100% {
    left: 100%;
  }
}

@keyframes myfirst {
  0% {
    left: -25%;
  }
  100% {
    left: 100%;
  }
}

/*************footer End*****************/
</style>

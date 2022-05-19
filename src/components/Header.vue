<template>
  <div>
    <div>
      <div>
            <b-navbar toggleable="lg" type="light" variant="white">
              <b-navbar-brand href="#">
                <b-img src="logo.png" style="height: 45px; width: 140px;"></b-img>
              </b-navbar-brand>
              <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
              <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                  <b-nav-item href="/#/">Home</b-nav-item>
                  <b-nav-item href="https://yubot.blogspot.com">Blog</b-nav-item>
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">
                </b-navbar-nav>
              </b-collapse>
            </b-navbar>
            <div class="container-banner">
                <h1 class='banner-header-text'>Yuviony 24*7  Online Tamil Radio</h1>
            </div>
          </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'Header',
}
</script>
<style>
 .navbar {
      margin-bottom: 0px;
  }

  .container-banner {
    height: 170px;
    color: #ffffff;
    font-size: 28px;
    font-weight: 400;
    text-shadow: thistle;
    text-align: inherit;
    background: rgb(2,0,36);
    background: linear-gradient(117deg, rgba(2,0,36,1) 0%, rgba(9,9,121,1) 46%, rgba(0,212,255,1) 100%);
}

.banner-header-text {
    font-size: 28px;
    text-transform: capitalize;
    color: white;
    padding: 3rem;
}

  .affix ~ .container-fluid {
     position: relative;
     top: 50px;
  }
.navbar-inverse {
    background-color: #fff;
    color: #000;
    font-color: #000;
    text-transform: capitalize;
    font-weight: Bold;
    font-size: 14px;
    border-bottom: 2px, solid, #000;
}

.navbar-nav {
   text-transform: capitalize;
   color: #000;
   font-weight: Bold;
   }
.navbar-inverse .navbar-brand {
    color: #fff;
}
.nav>li>a:hover {
    text-decoration: none;
    background-color: #fff;
    font-size: 18px;
    font-color: #000;
}
.navbar-inverse .navbar-nav>li>a {
    color: #000;
}

</style>



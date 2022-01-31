<template>
  <div>
    <div class='container-fluid' id='header-background' style='height:95px;'>
      <b-img src="logo.png" fluid alt="Yuviony"></b-img>
    </div>
    <div>
      <b-navbar toggleable="lg" type="dark" fixed="true" class="navbar navbar-inverse">
        <b-navbar-brand href="#">Yuviony</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="/">Home</b-nav-item>
            <b-nav-item href="https://yubot.blogspot.com/">News</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
</div>
</template>

<script>
export default {
  name: 'Header',
}
</script>
<style>
#header-background {
    height: 55px;
    background: #C2185B;
    background: -webkit-linear-gradient(#C2185B, #E91E63);
    background: -o-linear-gradient(#C2185B, #E91E63);
    background: -moz-linear-gradient(#C2185B, #E91E63);
    background: linear-gradient(#C2185B, #E91E63);
   }

#header-bck {
    height: 55px;
    background: #fff;
   }

  .affix {
      top:0;
      width: 100%;
      z-index: 9999 !important;
  }
 .navbar {
      margin-bottom: 0px;
      font-color: #fff;
  }

  .affix ~ .container-fluid {
     position: relative;
     top: 50px;
  }
.navbar-inverse {
    background-color: #C51162;
    color: #fff;
    text-transform: UPPERCASE;
    font-color: #fff;
    font-weight: Bold;
    font-size: 14px;
}

.navbar-nav {
   text-transform: UPPERCASE;
   color: #fff;
   font-weight: Bold;
   font-color: #fff;
   }
.navbar-inverse .navbar-brand {
    color: #fff;
}
.nav>li>a:hover {
    text-decoration: none;
    background-color: #fff;
    font-size: 18px;
    font-color: #fff;
}
.navbar-inverse .navbar-nav>li>a {
    color: #fff;
}

</style>



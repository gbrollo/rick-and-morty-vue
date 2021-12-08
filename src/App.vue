<template>
  <div class="gio-main">
    <div class="bg"></div>
    <div class="header">

      <router-link class="link" to="/characters">Characters</router-link>
      <router-link class="link" to="/episodes">Episodes</router-link>
      <router-link class="link" to="/locations">Locations</router-link>

      <button class="menu">M</button>

      <div class="nav-logo">
        <router-link to="/">
          <img style="max-height: 100%" src="src/assets/rick_and_morty.png" alt="Rick and Morty" />
        </router-link>
      </div>

    </div>
    <div class="gio-content">
      <transition name="page-fade">
        <router-view/>
      </transition>
    </div>
    <div class="footer">
        <div class="footer-img">
          <img style="max-height:200px" src="/src/assets/rick_and_morty_foff.png" alt="" />
        </div>
    </div>    
  </div>
</template>

<script>
import { routes } from './routes';

export default {
  components: {
  },
  data () {
    return {
      routes
    }
  }
}
</script>

<style>
  html {
    font-family: Helvetica, sans-serif;
  }
  body {
    background-color: #1f1c3c;
    margin: 0;
  }

  .header {
    height: 60px;
    position: relative;
    overflow: hidden;
    background-color: #1d152ee3;
    padding: 5px;
  }
  .header a.link {
    float: left;
    color: #73d361;
    text-align: center;
    padding: 0px 16px;
    text-decoration: none;
    font-size: 17px;
    line-height: 60px;
    text-transform: uppercase;
  }
  .header a:hover {
    background-color: #20162e;
    color: #21a1bb;
  }
  .header .nav-logo {
    height: 60px;
    float: none;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .bg {
    background: url("./assets/background.jpg") center center;
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: cover; /* Resize the background image to cover the entire container */
    position: absolute;
    z-index: -1;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    opacity: .4;
      width: 100%;
      height: 100%;
  }
  .gio-content {
    min-height: calc(100vh - 230px);
    background-color: #1f1c3c73;
    margin: 30px;
    overflow: auto;
    max-height: calc(100vh - 150px);
  }
  .footer {
    height: 200px;
    background: #21a1bb;
    bottom: 0;
    border-left: 98vw solid #21a1bb;
  }
  .footer-img {
    position: absolute;
    z-index: 999;
    left: 0;
  }

  .header button.menu {
    display: none;
  }

  @media only screen and (max-width: 880px) {
    .header a {
      display: none
    }
    .header button.menu {
      display: block;
    }
  }

  .page-fade-enter-active, .page-fade-leave-active {
    transition: opacity .5s;
  }
  .page-fade-enter, .page-fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
    opacity: 0;
  }

/* width */
::-webkit-scrollbar {
  width: 6px;
  height: 6px;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px #1d152ee3; 
  border-radius: 10px;
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: #55a43d; 
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #55a43d; 
}
</style>

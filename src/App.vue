<template>
  <div class="gio-main">
    <div class="gio-content">
      <transition name="pagina-fade">
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
  body {
    background-color: #1f1c3c;
    margin: 0;
  }
  .gio-content {
    min-height: calc(100vh - 230px);
  }
  .footer {
    height: 200px;
    background: #21a1bb;
    bottom: 0;
    border-top: 30px solid #1f1c3c;
    border-left: 98vw solid #21a1bb;
  }
  .footer-img {
    position: absolute;
    z-index: 999;
    left: 0;
  }
</style>

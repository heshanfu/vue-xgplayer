<template>
  <div id="app">
    <div class="my-5">
      <span class="badge badge-light">Github</span>
      <a href="http://github.com/savokiss/vue-xgplayer" target="_blank">
        <img src="https://img.shields.io/github/stars/savokiss/vue-xgplayer.svg?style=social" alt="">
      </a>
    </div>
    <h3>Vue xgplayer</h3>
    <div class="container mt-5">
      <xgplayer class="xgplayer" :options="playerOptions"></xgplayer>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      playerOptions: {
        url: 'https://h5player.bytedance.com/video/mp4/xgplayer-demo-360p.mp4',
        poster: '//s2.pstatp.com/cdn/expire-1-M/byted-player-videos/1.0.0/poster.jpg'
      }
    }
  }
}
</script>

<style>
@import url('https://cdn.bootcss.com/bootstrap/4.1.1/css/bootstrap.min.css');
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.xgplayer {
  margin: 0 auto;
}
</style>

<template>
  <div>
    <HeaderPage/>
    <b-container fluid>
      <div class="ad-container">
        <Adsense
          data-ad-client="ca-pub-2464991287215606"
          data-ad-slot="1146494313"
          data-ad-format="auto"
          :data-full-width-responsive="true"
        >
        </Adsense>
      </div>
    </b-container>
    <b-container fluid>
      <b-card
        border-variant="info"
        header-border-variant="info"
        header-text-variant="info"
        align="center"
      >
        <b-card-text>
          <div v-if="!is_playing">
            <b-button pill variant="outline-success" v-bind:disabled="is_playing" @click="playMusic()">
              <b-icon icon="play-fill" variant="success"></b-icon>
            </b-button>
          </div>

          <div v-if="is_playing">
            <b-spinner variant="info" type="grow" label=""></b-spinner>
            <br />
            <b-button pill variant="outline-success" v-bind:disabled="is_pause" @click="pauseMusic()">
              <b-icon icon="pause-fill" variant="success"></b-icon>
            </b-button>
          </div>

        </b-card-text>
        </b-card>
      </b-container>

  </div>
  </template>

  <script>
  import HeaderPage from '@/components/Header.vue';
  var myTrack = new Audio(require('@/assets/music/1.mp3'))
export default {
  name: 'HomePage',
  data() {
    return {
      is_playing: false,
      src: require('../assets/yuvionylogo.png'),
    }
  },
  methods: {
    playMusic() {
      this.is_playing = true;
      myTrack.play();
    },
    pauseMusic() {
      this.is_playing = false;
      myTrack.pause();
    }
  },
  components: {
    HeaderPage,
  },
}
</script>



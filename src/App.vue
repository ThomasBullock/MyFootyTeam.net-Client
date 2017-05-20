<template>
  <div id="app"> 
    <MainHeader></MainHeader>
    <StatsBar></StatsBar>
    <div class="container">
      <div class="row">
        <Squad></Squad>
        <PlayerList></PlayerList>  
      </div>      
    </div>

    
  </div>
</template>

<script>

// import {players} from './data/EssPlayerList';

import MainHeader from './components/MainHeader.vue';
import StatsBar from './components/StatsBar.vue';
import Squad from './components/Squad.vue';
import PlayerList from './components/PlayerList.vue';


export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    MainHeader,
    StatsBar,
    PlayerList,
    Squad

  }
}
</script>

<style lang="scss">
  @import "./assets/bootstrap-4.0.0-alpha.6/scss/bootstrap-custom.scss";
  @import './assets/scss/main.scss';

</style>

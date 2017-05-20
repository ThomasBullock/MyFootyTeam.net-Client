<template>
  <div id="app"> 
    <MainHeader></MainHeader>

    <main class="container">
      <div class="row">
        <StatsBar></StatsBar>
        <Squad></Squad>
        <div class="col-md-3 team">
          <PlayerDetail></PlayerDetail>
          <PlayerList></PlayerList>            
        </div>

      </div>      
    </main>

    
  </div>
</template>

<script>

// import {players} from './data/EssPlayerList';

import MainHeader from './components/MainHeader.vue';
import StatsBar from './components/StatsBar.vue';
import Squad from './components/Squad.vue';
import PlayerList from './components/PlayerList.vue';
import PlayerDetail from './components/PlayerDetail.vue';


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
    PlayerDetail,
    Squad

  }
}
</script>

<style lang="scss">
  @import "./assets/bootstrap-4.0.0-alpha.6/scss/bootstrap-custom.scss";
  @import './assets/scss/main.scss';

  main {
    padding-top: 47px;
  }

  .team {
    padding-top: 1em;
    padding-bottom: 1em;
    background: #AAA;
    border: 1px solid #555;       
  }


</style>

<template>
	<div class="col-sm-4">
		<ul>
		 	<li v-for="(value, key, index) in players">
		    <span>{{value.number}}</span><span>{{ key }}</span>
		  </li>		
		</ul>		
	</div>


</template>
<script>
	import players from '../data/EssPlayerList.json'; 

	export default {
  data: function() {
    return {
      players: players
    };
  },
  methods: {
  	clicky() {
  		console.log(this.players);
  	}
  }
}
</script>
<style lang="scss">
	ul {
		list-style: none;
	}

	li {
		display: flex;
		justify-content: space-between;
	}

</style>
<template>
	<div class="list-col">
		<ul class="playerlist">
		 	<li class="playerlist__item" v-for="(value, key, index) in players">
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
  @import '../assets/scss/main.scss';

	.list-col {
		// height: 200px;
		overflow: auto;
	}

	.playerlist {
		padding: 0;
		width: 100%;	
		background: #111;
	 	border: 1px solid #555; 
	 	display: flex;
	 	flex-direction: column;
	 	align-items: center;

	 	@include elem('item') {
			border: 1px solid darkred;		
			width: 80%;

			&:hover {
				background-color: darkred;
				border: 1px dashed crimson;				
			}
	 	}

		
		// .over {

		// }

	}


		// li {
		// 	display: flex;
		// 	justify-content: space-between;
		// }

</style>
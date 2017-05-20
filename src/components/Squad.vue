<template>
	<div class="field col-md-7">
		<ul class="field__list">
		 	<li class="field__item" v-for="(position, i) in squad" v-if="i < 18">
		 		<h5>{{position.pos}}</h5>
		    <Position></Position>
		  </li>
		 	<li class="field__item--last" v-for="(position, i) in squad" v-if="i >= 18">
		 		<h5>{{position.pos}}</h5>
		    <Position></Position>
		  </li>		
		</ul>
	</div>
</template>
<script>
	import Position from './Position.vue';
	

	export default {
		data: function() {
			return {
				squad: [{id: "LBP", pos: "Back Pocket", status: false, player: null},
				{id: "FB", pos: "Full Back", status: false, player: null},
				{id: "RBP", pos: "Back Pocket", status: false, player: null},
				{id: "LHB", pos: "Half Back", status: false, player: null},
				{id: "CHB", pos: "Centre Half Back", status: false, player: null},
				{id: "RHB", pos: "Half Back", status: false, player: null},
				{id: "LW", pos: "Wing", status: false, player: null},
				{id: "C", pos: "Center", status: false, player: null},	
				{id: "RW", pos: "Wing", status: false, player: null},
				{id: "LHF", pos: "Half Forward", status: false, player: null},
				{id: "CHF", pos: "Centre Half Forward", status: false, player: null},
				{id: "RHF", pos: "Half Forward", status: false, player: null},
				{id: "LFP", pos: "Forward Pocket", status: false, player: null},
				{id: "FF", pos: "Full Forward", status: false, player: null},
				{id: "RHP", pos: "Forward Pocket", status: false, player: null},
				{id: "Ruck", pos: "Ruck", status: false, player: null},
				{id: "RR", pos: "Ruck-Rover", status: false, player: null},
				{id: "Rover", pos: "Rover", status: false, player: null},
				{id: "IC-1", pos: "Bench", status: false, player: null},	
				{id: "IC-2", pos: "Bench", status: false, player: null},	
				{id: "IC-3", pos: "Bench", status: false, player: null},
				{id: "IC-4", pos: "Bench", status: false, player: null}]				
			}

		},
		components: {
			Position
		}
	}
</script>
<style lang="scss">
	@import '../assets/scss/main.scss';
	
	.field {

		background: url('../assets/img/Oval.jpg'), $charcoal;


		position: relative;
		margin: 0 auto 2em;	
		width: 680px;
		padding-top: 50px;
		padding-left: 0;
		padding-right: 0;
		padding-bottom: 5px;
		background-repeat: no-repeat;
		background-size: contain;
		background-position: center top;
		box-shadow: 0 1.5px 0 0 rgba(0,0,0,0.1);
		border: 1px solid #555;	
	
		@include elem('list') {
			list-style: none;
			display: flex;
			flex-wrap: wrap;
			justify-content: space-around;		
		}

		@include elem('item') {
			flex: 1 1 33%;		
			display: flex;
			flex-direction: column;
			align-items: center;

			@include mod('last') {
				flex: 1 1 25%;
				display: flex;
				flex-direction: column;
				align-items: center;				
			}

		}


	}

</style>
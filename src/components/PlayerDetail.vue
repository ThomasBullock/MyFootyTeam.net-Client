<template>
	<div class="player-detail">
		<h2>Player Detail</h2>
		<div class="player-detail__status">
			<button class="btn">Full list</button>
			<button class="btn">Available</button>
			<button class="btn" >Unavailable</button>
		</div>
		<div class="image-wrapper">
			<img class="img-fluid" src="../assets/img/BEGLEY Joshua.png" alt="">
		</div>
		<div class="player-detail__data">
			<table class="table table-sm table-inverse">
			  <tbody>
			    <tr>
			    	<th colspan="4">Joshua Begley</th>
			    </tr>			  
			    <tr>
			      <td>Age: </td>
			      <td>Ht: </td>
			      <td>Games: </td>
			    </tr>
			    <tr>
			    	<th colspan="4">This Year</th>
			    </tr>
			    <tr>
			      <td>Games: </td>
			      <td>Goals: </td>
			      <td>Fantasy: </td>
			    </tr>
			    <tr>
			    	<th colspan="4">Averages</th>
			    </tr>
			    <tr>
			      <td>Disp: </td>
			      <td>Tack: </td> 
			      <td>Disp Eff: </td>
			      <td>1%'s: </td>			      
			    </tr>
			  </tbody>
			</table>					
		</div>

	</div>
</template>

<script>
	
</script>

<style lang="scss">
	@import '../assets/scss/main.scss';

	.player-detail {

		@include elem('status') {
			display: flex;
			justify-content: space-between;

			button {
				padding: .25rem .5rem;
			}
		}

		@include elem('data') {
			display: flex;
			flex-wrap: wrap;
			// justify-content: space-between;
			span {
				margin-right: 2.5%;
				// flex: 0 1 45%;
			}
		}

	}
</style>
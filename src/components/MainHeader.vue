<template>
    <header class="navbar fixed-top navbar-inverse bg-inverse">
      <div class="container">
          <div class="row">
	          <h1 id="title" class="navbar-text">My Bomber Squad</h1>
	          <button id="clear-btn" type="button" class="btn">Clear Field</button>
	          <button id="save-btn" type="button" class="btn">Save PNG</button>
	          <button id="help" type="button" class="btn">?</button>
          </div>     
      </div>
    </header> 	
</template>

<script>

</script>

<style lang="scss">
  @import '../assets/scss/main.scss';

  header {
  	background: $oil;
  	position: fixed;
  	width: 100%;
    box-shadow: 0 2px 1px $black;
  }

	h1.navbar-text {
		color: $base;
		font-size: ms(2);
		margin-right: 1rem;
	}


</style>
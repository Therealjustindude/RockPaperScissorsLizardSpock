<script setup lang="ts">
import LizardPiece from '../game-pieces/LizardPiece.vue';
import PaperPiece from '../game-pieces/PaperPiece.vue';
import RockPiece from '../game-pieces/RockPiece.vue';
import ScissorsPiece from '../game-pieces/ScissorsPiece.vue';
import SpockPiece from '../game-pieces/SpockPiece.vue';

</script>

<template>
  <div id="step-one">
		<img alt="pentagon-bg" id="pentagon-bg" src="@/assets/bg-pentagon.svg" />
		<div id="top" class="piece-wrapper">
      <ScissorsPiece />
    </div>
    <div id="top-right" class="piece-wrapper">
      <PaperPiece />
    </div>
    <div id="bottom-right" class="piece-wrapper">
      <RockPiece />
    </div>
    <div id="bottom-left" class="piece-wrapper">
      <LizardPiece />
    </div>
    <div id="top-left" class="piece-wrapper">
      <SpockPiece />
    </div>
  </div>
</template>

<style scoped>
/* Parent Container */
#step-one {
	position: relative;
	display: flex;
	justify-content: center;
	align-items: center;
	height: 260px;
	width: 270px;
}

/* Pentagon Background */
#pentagon-bg {
	height: 100%;
	width: 100%;
}

.piece-wrapper {
	position: absolute;
}

#top {
	top: -16%;
	left: 35%;
}

#top-left {
	top: 24%;
	left: -11%;
}

#top-right {
	top: 24%;
	left: 80%;
}

#bottom-left {
	top: 82%;
	left: 5%;
}

#bottom-right {
	top: 82%;
	right: 5%;
}

/* For desktops (screens larger than 1024px) */
@media (min-width: 600px) { 
	#step-one {
		height: 390px; 
		width: 400px; 
	}

	#top {
		top: -16%;
		left: 35%;
	}

	#top-left {
		top: 24%;
		left: -10%;
	}
	
	#top-right {
		top: 24%;
		left: 80%;
	}
	
	#bottom-left {
		top: 82%;
		left: 5%;
	}
	
	#bottom-right {
		top: 82%;
		right: 5%;
	}
}
</style>

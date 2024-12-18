<script setup lang="ts">
</script>

<template>
  <div class="piece-outline-inital" id="scissor-piece">
		<div class="piece-bg-initial"> 
			<img alt="Scissor Icon" class="piece-icon" src="@/assets/icon-scissors.svg" />
		</div>
  </div>
</template>

<style scoped>
#scissor-piece {
	background: var(--color-primary-scissors);
	position: absolute;
	top: 0;
}
.piece-icon {
	height: 50%;
	width: 50%;
}
</style>

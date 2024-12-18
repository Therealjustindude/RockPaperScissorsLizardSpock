<script setup lang="ts">
</script>

<template>
  <div class="piece-outline-inital" id="lizard-piece">
		<div class="piece-bg-initial"> 
			<img alt="Lizard Icon" class="piece-icon" src="@/assets/icon-lizard.svg" />
		</div>
  </div>
</template>

<style scoped>
#lizard-piece {
	background: var(--color-primary-lizard);
	position: absolute;
	top: 0;
}
.piece-icon {
	height: 50%;
	width: 50%;
}
</style>

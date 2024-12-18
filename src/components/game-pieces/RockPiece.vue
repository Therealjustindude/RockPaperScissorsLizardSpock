<script setup lang="ts">
</script>

<template>
  <div class="piece-outline-inital" id="rock-piece">
		<div class="piece-bg-initial"> 
			<img alt="Rock Icon" class="piece-icon" src="@/assets/icon-rock.svg" />
		</div>
  </div>
</template>

<style scoped>
#rock-piece {
	background: var(--color-primary-rock);
}

.piece-icon {
	height: 50%;
	width: 50%;
}
</style>

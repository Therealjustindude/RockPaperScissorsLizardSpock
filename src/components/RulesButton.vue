<script setup lang="ts">
  defineProps<{
    msg?: string
  }>()
</script>

<template>
  <button id="rules-button">
    <p>RULES</p>
  </button>
</template>

<style scoped>
	#rules-button {
		background: none;
		border: 1px solid white;
		border-radius: 10px;
		padding: 8px;
		width: 128px;
		height: 40px;
		cursor: pointer;
	}

	#rules-button p {
		color: white;
		font-size: medium;
		font-weight: 500;
	}
</style>

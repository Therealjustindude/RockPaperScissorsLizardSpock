<script setup lang="ts">
import StepOne from './steps/StepOne.vue';

</script>

<template>
  <div id="game-board">
    <StepOne />
  </div>
</template>

<style scoped>
#game-board {
  display: flex;
	justify-content: center;
	align-items: center; 
}
</style>

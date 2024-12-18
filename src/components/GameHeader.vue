<script setup lang="ts">
  import ScoreCard from './ScoreCard.vue';
</script>

<template>
  <div id="game-header">
		<img alt="Game logo" id="logo" src="@/assets/logo-bonus.svg" />
		<ScoreCard />
	</div>
</template>

<style scoped>
#logo {
  width: 80px; 
  height: 80px;
}

#game-header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  border: 4px solid var(--color-neutral-header-outline);
  border-radius: 10px;
  width: 90%;
  padding: 8px 16px;
}

/* For desktops (screens larger than 1024px) */
@media (min-width: 1024px) {
  #logo {
    width: 125px; 
    height: 125px;
  }

  #game-header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    border: 4px solid var(--color-neutral-header-outline);
    border-radius: 10px;
    width: 60%;
    padding: 16px 32px;
  }
}
</style>

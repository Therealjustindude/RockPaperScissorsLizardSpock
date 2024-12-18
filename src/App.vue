<script setup lang="ts">
  import HelloWorld from './components/HelloWorld.vue'
  import RulesButton from './components/RulesButton.vue';
import ScoreCard from './components/ScoreCard.vue';
</script>

<template>
  <header>
    <div id="game-header">
      <img alt="Game logo" class="logo" src="@/assets/logo-bonus.svg" width="125" height="125" />
      <ScoreCard />
    </div>
  </header>
  <main>
    <HelloWorld msg="You did it!" />
  </main>
  <footer>
    <RulesButton />
  </footer>
</template>

<style scoped>
header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  padding: 32px;
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

footer {
  position: absolute;
  bottom: 0;
  display: flex;
  justify-content: flex-end;
  width: 100%;
  margin-bottom: 32px;
  padding-right: 32px;
}
</style>

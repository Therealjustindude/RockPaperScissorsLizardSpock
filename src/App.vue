<script setup lang="ts">
  import HelloWorld from './components/HelloWorld.vue'
  import RulesButton from './components/RulesButton.vue';
import ScoreCard from './components/ScoreCard.vue';
</script>

<template>
  <header>
    <div id="game-header">
      <img alt="Game logo" id="logo" src="@/assets/logo-bonus.svg" />
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

main {
  margin-left: auto;
  margin-right: auto;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

footer {
  position: absolute;
  bottom: 0;
  display: flex;
  justify-content: center;
  width: 100%;
  margin-bottom: 48px;
}

/* For desktops (screens larger than 1024px) */
@media (min-width: 1024px) {
  header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding: 32px;
  }

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

  footer {
    position: absolute;
    bottom: 0;
    display: flex;
    justify-content: flex-end;
    width: 100%;
    margin-bottom: 32px;
    padding-right: 32px;
  }
}
</style>

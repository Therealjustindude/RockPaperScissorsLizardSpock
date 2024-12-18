<script setup lang="ts">
import GameHeader from './components/GameHeader.vue'; 
import RulesButton from './components/RulesButton.vue';
import GameBoard from './components/GameBoard.vue';
</script>

<template>
  <div id="layout">
    <header>
      <GameHeader />
    </header>
    <main>
      <GameBoard/>
    </main>
    <footer>
      <RulesButton />
    </footer>
  </div>
</template>

<style scoped>
#layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* Full viewport height */
  min-width: 100vw; /* Full viewport height */
}
header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  padding: 32px;
}

main {
  display: flex;
  flex: 1;
  width: 100%;
  height:100%;
  align-items: center;
  justify-content: center;
}

footer {
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
    display: flex;
    justify-content: flex-end;
    width: 100%;
    margin-bottom: 32px;
    padding-right: 32px;
  }
}
</style>

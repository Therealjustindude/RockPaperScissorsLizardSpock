<script setup lang="ts">
</script>

<template>
  <div id="score-card">
    <p id="score-title">SCORE</p>
    <p id="user-score">01</p>
  </div>
</template>

<style scoped>
#score-card {
  background-color: white;
  border-radius: 10px;
  width: 6rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
#score-title {
  color: var(--color-neutral-dark-text);
  font-size: x-small;
  font-weight: 200;
}
#user-score {
  color: var(--color-neutral-dark-text);
  font-size: x-large;
  font-weight: 900;
}

/* For desktops (screens larger than 1024px) */
@media (min-width: 1024px) { 
  #score-card {
    background-color: white;
    border-radius: 10px;
    width: 10rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  #score-title {
    color: var(--color-neutral-dark-text);
    font-size: large;
    font-weight: 500;
  }
  #user-score {
    color: var(--color-neutral-dark-text);
    font-size: 60px;
    font-weight: bolder;
  }
}
</style>

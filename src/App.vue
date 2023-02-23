<script setup>
// import Valorant from './components/teste.vue';
// <!-- <Valorant mortes="216" /> -->
import Header from './components/Header.vue'
import Persona from './components/Persona.vue'
import Choice from './components/Choice.vue'
      fetch("../mock/personas.json")
        .then((response) => response.json())
        .then((json) => {
            persona:Object
        })
        // }
</script>

<template>
  <div class="body">
    <div class="main">
      <Header/>
      <Persona Object/>
      <Choice/>
  </div>
</div>
</template>

<style scoped>
.body {
  height: auto;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--color-body);
  background: url("./assets/img/wallpapers3.png") no-repeat;
  background-size: cover;
  font-family: "Roboto", sans-serif;
}
.main {
  height: auto;
  width: 90vw;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
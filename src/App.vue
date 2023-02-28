<script setup>
// import Valorant from './components/teste.vue';
// <!-- <Valorant mortes="216" /> -->
import Header from "./components/Header.vue";
import Persona from "./components/Persona.vue";
import Choice from "./components/Choice.vue";
import jsonPersonas from "./mock/personas.json";
</script>

<template>
  <div class="body">
    <div class="main">
      <Header />
      <Persona
        v-for="item in jsonPersonas"
        :key="item.title"
        :title="item.title"
        :image="item.image"
        :matches="item.matches"
        :victories="item.victories"
        :defeats="item.defeats"
        :headshots="item.headshots"
        :winrate="item.winrate"
        :slaughter="item.slaughter"
        :deaths="item.deaths"
        :assists="item.assists"
        :kills="item.kills"
        :kda="item.kda"
        :skill_1="item.skill_1"
        :skill_2="item.skill_2"
        :skill_3="item.skill_3"
        :skill_4="item.skill_4"
        :history="item.history"
        :quality="item.quality"
        :description="item.description"
      />
      <Choice />
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

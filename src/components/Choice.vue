<template>
    <section class="personas-bottom">
      <div class="division">
        <div class="plane-line"></div>
        <div class="arrow">
          <img src="./assets/icons/seta.png" alt="Seta dupla " />
        </div>
        <div class="plane-line"></div>
      </div>
      <div class="choice-persona">
        <img
          src="./assets/img/e.p 1 (Cypher).png"
          alt="Personagem Cypher"
          />
          <img src="./assets/img/e.p 2 (Omi).png" alt="Personagem Omi" />
          <img src="./assets/img/e.p 3 (Astra).png" alt="Personagem Astra" />
          <img src="./assets/img/e.p 4 (Viper).png" alt="Personagem Viper" />
          <img
          src="./assets/img/e.p 5 (Chambito).png"
          alt="Personagem Chambito"
          />
          <img src="./assets/img/e.p 6 (Yoru).png" alt="Personagem Yoru" />
          <img src="./assets/img/e.p 7 (Sova).png" alt="Personagem Sova" />
          <img
          class="image-reyna"
          src="./assets/img/e.p 8 (Reyna).png"
          alt="Personagem Reyna"
          />
          <img src="./assets/img/e.p 9(KJ).png" alt="Personagem KJ" />
          <img src="./assets/img/e.p 10(Kay-o).png" alt="Personagem Kay-o" />
          <img src="./assets/img/e.p 11(Jett).png" alt="Personagem Jett" />
          <img src="./assets/img/e.p 12(Sage).png" alt="Personagem Sage" />
          <img src="./assets/img/e.p 13(Neon).png" alt="Personagem Neon" />
          <img src="./assets/img/e.p 14(Brit).png" alt="Personagem Brit" />
          <img
          src="./assets/img/e.p 15(Boneco novo).png"
          alt="Personagem Boneco novo"
        />
      </div>
    </section>
</template>

<style scoped>

.personas-bottom {
  width: 60vw;
  height: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  /* border-top: solid 1px var(--color-body); */
  flex-direction: column;
}

.personas-bottom .division {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 15px;
}

.division .plane-line {
  border: solid 1px var(--color-plane);
  height: 0px;
  width: 31vw;
}
.personas-bottom .choice-persona {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 12px;
}

.choice-persona .image-reyna {
  margin-bottom: 15px;
}

.choice-persona img {
  transition: .4s;
  cursor: context-menu !important; 

}
.choice-persona:hover > :not(:hover) {
  opacity: .4;
  transform: scale(.9);
}

</style>
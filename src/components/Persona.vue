<script setup>
    defineProps({
        persona:Object,
        title:String,
        image:String,
        matches:String,
        victories: String,
        defeats:String,
        headshots:String,
        winrate:String,
        slaughter:String,
        deaths:String,
        assists:String,
        kills:String,
        kda:String,
        skill_1:String,
        skill_2:String,
        skill_3:String,
        skill_4:String,
        history:String,
        quality:String,
        description:String
    })
    
</script>
<template>
  <section class="center">
    <div class="center-left">
      <div class="center-left-title">
        <p>Estatísticas com o agente</p>
        <h1>RESUMO</h1>
      </div>
      <div class="center-left-information">
        <div class="center-left-inf-left">
          <ul>
            <li>
              <p>Partidas jogadas</p>
              <span>{{matches}} partidas</span>
            </li>
            <li>
              <p>Vitórias</p>
              <span> {{ victories}} vitórias</span>
            </li>
            <li>
              <p>Derrotas</p>
              <span> {{ defeats}}Derrotas</span>
            </li>
            <li>
              <p>Tiros na cabeça</p>
              <span> {{ headshots}} tiros na cabeça</span>
            </li>
            <li>
              <p>Winrate</p>
              <span> {{ winrate}} %</span>
            </li>
          </ul>
        </div>
        <div class="center-left-inf-right">
          <ul>
            <li>
              <p>Abates</p>
              <span> {{ slaughter}} abates</span>
            </li>
            <li>
              <p>Mortes</p>
              <span>{{ deaths }} mortes</span>
            </li>
            <li>
              <p>Assistências</p>
              <span>{{ assists }} assistências</span>
            </li>
            <li>
              <p>Headshot/kills</p>
              <span> {{ kills }} abates na cabeça</span>
            </li>
            <li>
              <p>KDA</p>
              <span>{{ kda }} %</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="center-shadow-persona">
      <h1>{{ title }}</h1>
      <img
        src="../assets/icons/fundo  reyna.png"
        alt="Imagem da personagem Reyna"
      />
    </div>
    <div class="image-persona">
      <img src={{ image }} alt="image-persona" />
    </div>
    <div class="center-right">
      <div class="center-right-title">
        <p>{{ quality }}</p>
        <h1>HABILIDADES</h1>
      </div>
      <div class="center-right-skills">
        <img {{skill_1}}/>
        <img {{skill_2}}/>
        <img {{skill_3}}/>
        <img {{skill_4}}/>
        <!-- <img
          src="../assets/img/habilidade 2.png"
          alt="Imagem habilidade 2 da personagem Reyna"
        />
        <img
          src="../assets/img/habilidade 3.png"
          alt="Imagem habilidade 3 da personagem Reyna"
        />
        <img
          src="../assets/img/habilidade 4.png"
          alt="Imagem habilidade 4 da personagem Reyna"
        />
        <img
          src="../assets/img/habilidade 5.png"
          alt="Imagem habilidade 5 da personagem Reyna"
        /> -->
      </div>
      <div class="center-right-texts">
        <span> {{ history }}</span
        >
        <div class="explication">
          <h3>{{ quality }}</h3>
          <p> {{ description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.center {
  width: 100%;
  height: 100%;
  display: flex;
  /* border: solid 1px var(--color-body); */
  padding-top: 100px;
  align-items: center;
}

.center-left {
  width: 33.3%;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-right: solid 1px var(--color-body);
  padding-right: 20px;
}

.center-left .center-left-title {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  padding-right: 30px;
}

.center-left .center-left-title p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
}

.center-left .center-left-title h1 {
  font-weight: 600;
  font-size: 36px;
  line-height: 42px;
  color: var(--resumo-titulo);
}

.center-left .center-left-information {
  display: flex;
  flex-direction: row;
  /* border: solid 1px green; */
  justify-content: end;
  padding-top: 20px;
}

.center-left .center-left-inf-left ul {
  display: flex;
  flex-direction: column;
  gap: 20px;
  text-align: left;
  list-style-type: none;
  /* border: solid 1px red; */
  width: 8vw;
}

.center-left .center-left-inf-left li p {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.center-left .center-left-inf-left li span:hover {
  color: var(--color-plane);
}

.center-left .center-left-inf-left li span {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  color: var(--resumo-titulo);
}

.center-left .center-left-inf-right ul {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
  gap: 20px;
  text-align: right;
  list-style-type: none;
  width: 8vw;
}

.center-left .center-left-inf-right li p {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.center-left .center-left-inf-right li span {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  color: var(--resumo-titulo);
}

.center-left .center-left-inf-right li span:hover {
  color: var(--color-plane);
}

.center .center-shadow-persona {
  width: 33.3%;
  height: 70vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.center .center-shadow-persona h1 {
  font-weight: 700;
  font-size: 96px;
  line-height: 112px;
  padding-top: 80px;
}

.center .center-shadow-persona img {
  display: flex;
  position: relative;
  bottom: 20%;
  left: 0;
  border-bottom: solid 1px var(--color-body);
}

.center .image-persona img {
  position: absolute;
  right: 42%;
  top: 28%;
}

.center .center-right {
  width: 33.3%;
  height: 3auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-left: solid 1px var(--color-body);
  gap: 1vw;
  padding-left: 20px;
}

.center-right .center-right-title {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 1px;
}

.center-right .center-right-title p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
}

.center-right .center-right-title h1 {
  font-weight: 600;
  font-size: 36px;
  line-height: 42px;
  color: var(--resumo-titulo);
}

.center-right .center-right-skills {
  display: flex;
  align-items: flex-start;
  gap: 1vw;
  position: relative;
}

.center-right .center-right-skills img:hover {
  transform: scale(1.1);
}

.center-right .center-right-texts {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.center-right .center-right-texts span {
  color: #f9aff6;
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  width: 15vw;
  text-align: justify;
}

.center-right .center-right-texts h3 {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.center-right .center-right-texts p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  width: 14vw;
}

.center-right .center-right-texts .explication {
  gap: 10px;
}
</style>

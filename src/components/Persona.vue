<script setup>
    defineProps({
        persona:Object
    })
    
</script>
<template>
  <section class="centro">
    <div class="centro-esquerda">
      <div class="centro-esquerda-titulo">
        <p>Estatísticas com o agente</p>
        <h1>RESUMO</h1>
      </div>
      <div class="centro-esquerda-informacoes">
        <div class="centro-esquerda-inf-e">
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
        <div class="centro-esquerda-inf-d">
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
    <div class="centro-sombra-personagem">
      <h1>{{ title }}</h1>
      <img
        src="../assets/icons/fundo  reyna.png"
        alt="Imagem da personagem Reyna"
      />
    </div>
    <div class="img-personagem">
      <img src="../assets/img/personagem 2.png" alt="" />
    </div>
    <div class="centro-direita">
      <div class="centro-direita-titulo">
        <p>{{ quality }}</p>
        <h1>HABILIDADES</h1>
      </div>
      <div class="centro-direita-habilidades">
        <img
          src="../assets/img/habilidade 1.png"
          alt="Imagem habilidade 1 da personagem Reyna"
        />
        <img
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
        />
      </div>
      <div class="centro-direita-textos">
        <span> {{ history }}</span
        >
        <div class="explicacao-duelista">
          <h3>{{ quality }}</h3>
          <p> {{ description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.centro {
  width: 100%;
  height: 100%;
  display: flex;
  /* border: solid 1px var(--color-body); */
  padding-top: 100px;
  align-items: center;
}

.centro-esquerda {
  width: 33.3%;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-right: solid 1px var(--color-body);
  padding-right: 20px;
}

.centro-esquerda .centro-esquerda-titulo {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  padding-right: 30px;
}

.centro-esquerda .centro-esquerda-titulo p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
}

.centro-esquerda .centro-esquerda-titulo h1 {
  font-weight: 600;
  font-size: 36px;
  line-height: 42px;
  color: var(--resumo-titulo);
}

.centro-esquerda-informacoes {
  display: flex;
  flex-direction: row;
  /* border: solid 1px green; */
  justify-content: end;
  padding-top: 20px;
}

.centro-esquerda-inf-e ul {
  display: flex;
  flex-direction: column;
  gap: 20px;
  text-align: left;
  list-style-type: none;
  /* border: solid 1px red; */
  width: 8vw;
}

.centro-esquerda-inf-e li p {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.centro-esquerda-inf-e li span:hover {
  color: var(--color-plane);
}

.centro-esquerda-inf-e li span {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  color: var(--resumo-titulo);
}

.centro-esquerda-inf-d ul {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
  gap: 20px;
  text-align: right;
  list-style-type: none;
  /* border: solid 1px red; */
  width: 8vw;
}

.centro-esquerda-inf-d li p {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.centro-esquerda-inf-d li span {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  color: var(--resumo-titulo);
}

.centro-esquerda-inf-d li span:hover {
  color: var(--color-plane);
}

.centro-sombra-personagem {
  width: 33.3%;
  height: 70vh;
  display: flex;
  flex-direction: column;
  /* border: solid 1px var(--color-body); */
  justify-content: center;
  align-items: center;
  /* padding-bottom: 100px; */
}

.centro-sombra-personagem h1 {
  font-weight: 700;
  font-size: 96px;
  line-height: 112px;
  padding-top: 80px;
}

.centro-sombra-personagem img {
  display: flex;
  position: relative;
  bottom: 20%;
  left: 0;
  border-bottom: solid 1px var(--color-body);
}

.img-personagem img {
  position: absolute;
  right: 42%;
  top: 28%;
}

.centro .centro-direita {
  width: 33.3%;
  height: 3auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-left: solid 1px var(--color-body);
  gap: 1vw;
  padding-left: 20px;
}

.centro-direita .centro-direita-titulo {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 1px;
}

.centro-direita .centro-direita-titulo p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
}

.centro-direita .centro-direita-titulo h1 {
  font-weight: 600;
  font-size: 36px;
  line-height: 42px;
  color: var(--resumo-titulo);
}

.centro-direita .centro-direita-habilidades {
  display: flex;
  align-items: flex-start;
  gap: 1vw;
  position: relative;
}

.centro-direita-habilidades img:hover {
  transform: scale(1.1);
}

.centro-direita .centro-direita-textos {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.centro-direita-textos span {
  color: #f9aff6;
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  width: 15vw;
  text-align: justify;
}

.centro-direita .centro-direita-textos h3 {
  font-weight: 700;
  font-size: 16px;
  line-height: 19px;
}

.centro-direita .centro-direita-textos p {
  font-weight: 300;
  font-size: 13px;
  line-height: 15px;
  width: 14vw;
}

.centro-direita-textos .explicacao-duelista {
  gap: 10px;
}
</style>

<template>
    <header>
        <div class="fundo-menu">
          <img src="../assets/icons/fundo menu.png" alt="" />
        </div>
        <div class="inicio-menu">
        <img src="../assets/icons/inicio menu.png" alt="" />
        <p>INÍCIO</p>
      </div>
      <div class="icons-e">
        <a href="/resume.html">
          <img src="../assets/icons/menu 1.png" alt="" />
        </a>
        <img src="../assets/icons/campeos branco.png" alt="" />
      </div>
      <div class="icons-d">
        <a href="/arsenal.html">
          <img src="../assets/icons/menu 3.png" alt="" />
        </a>
        <a href="/rank.html">
          <img src="../assets/icons/menu 4.png" alt="" />
        </a>
      </div>
    </header>
</template>

<style scoped>
header {
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
}

header .fundo-menu {
  position: relative;
  bottom: 84%;
}

header .inicio-menu {
  position: absolute;
  top: 0%;
  left: 45%;
}

header .inicio-menu a { 
  color: var(--color-body);
}

header .inicio-menu p {
  font-weight: 600;
  font-size: 28px;
  line-height: 33px;
  position: absolute;
  top: 2%;
  right: 30%;
}

header .icons-e {
  position: absolute;
  left: 39%;
  top: 0%;
}

.icons-e img {
  margin-right: 6px;
}

header .icons-d {
  position: absolute;
  right: 38%;
  top: 0%;
}
.icons-d img {
  margin-right: 6px;
}
</style>
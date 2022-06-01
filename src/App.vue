<template>
  <header class="menu-superior">
    <div class="menu-esquerdo">
      <span> Home </span>
      <span> | </span>
      <span> Times </span>
      <span> | </span>
      <span> Jogadores </span>
    </div>
    <div class="menu-direito">
      <span> Sair </span>
    </div>
  </header>

  <RouterView />
</template>

<style>
@import "@/assets/base.css";

header.menu-superior {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

#app {
  max-width: 1280px;
  margin: 0 auto;
  /* padding: 2rem; */
  height: 100vh;

  font-weight: normal;
}

/* h1 {
  transition: 0.25s;
  width: fit-content;
  color: rgb(0, 0, 0);
  cursor: pointer;
}

h1:hover {
  transform: matrix(1000, 70, 60, 50, 40, 30);
  color: black;
} */

header,
footer {
  background-color: crimson;
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}

header span {
  padding: 0% 20px;
}

.balls {
  transform: perspective(1 3 5 7);
}

main {
  height: 70%;
}
</style>

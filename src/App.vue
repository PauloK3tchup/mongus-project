<template>
  <header>
    Cabeçalho
  </header>
  <main>
    <h1>Among us jumpscare (very scary)</h1>
  </main>
  <footer>
    Rodapau
  </footer>
</template>

<style>
@import '@/assets/base.css';

#app {
  max-width: 1280px;
  margin: 0 auto;
  /* padding: 2rem; */
  height: 100vh;

  font-weight: normal;
}

h1{
  transition: 1.25s;
  width: fit-content;
  color: rgb(0, 0, 0);
  cursor: pointer;
}

h1:hover{
  transform: matrix(1000, 70, 60, 50, 40, 30);
  color: black;
}

header, footer{
  background-color: red;
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}

</style>
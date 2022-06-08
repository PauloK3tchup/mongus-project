<script>
export default {
  data() {
    return {
      times: [
        { id: 1, name: "Time 1" },
        { id: 2, name: "Time 2" },
        { id: 3, name: "Time 3" },
        { id: 4, name: "Time 4" },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
    <div class="form-input">
      <input type="text" name="" id="" placeholder="Nome do time" />
      <button>Salvar</button>
    </div>
    <div class="list-items">
      {{ times }}
      <table>
        <thead>
          <tr>
            <th>ID</th>
            <th>Nome</th>
            <th>Ações</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th>1</th>
            <th>Comunismo</th>
            <th>☭</th>
          </tr>
          <tr>
            <th>2</th>
            <th>Capitalismo</th>
            <th>$</th>
          </tr>
          <tr>
            <th>3</th>
            <th>Olavo de Carvalho</th>
            <th>☠</th>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  <div class="mrwhite">
    <img
      class="bobux"
      src="https://www.einerd.com.br/wp-content/uploads/2019/06/Walter-White-morreu-Breaking-Bad-capa.jpg"
      alt=""
    />
  </div>
</template>
<style scoped>
.mrwhite {
  display: flex;
  justify-content: center;
}

img.bobux {
  width: 1%;
  height: auto;
  transition: 0.1s;
  opacity: 0;
}

img.bobux:hover {
  transform: scale(100);
  opacity: 100%;
}
</style>

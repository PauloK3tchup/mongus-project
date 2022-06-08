<script>
export default {
  data() {
    return {
      jogadores: [
        { id: 1, name: "Jogador 1", n_camisa: 1, time: 1 },
        { id: 2, name: "Jogador 2", n_camisa: 2, time: 2 },
        { id: 3, name: "Jogador 3", n_camisa: 3, time: 3 },
        { id: 4, name: "Jogador 4", n_camisa: 4, time: 4 },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="title">
        <h2>Gerenciamento de Jogadores</h2>
      </div>
      <div class="form-input">
        <input type="text" name="" id="" placeholder="Nome do Jogador" />
        <input type="text" name="" id="" placeholder="Time" />
        <button>Salvar</button>
      </div>
      <div class="list-items">
        <table>
          <thead>
            <tr>
              <th>ID</th>
              <th>Nome</th>
              <th>N° Camisa</th>
              <th>Time ID</th>
              <th>Ações</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="jogador in jogadores" :key="jogador.id">
              <th>{{ jogador.id }}</th>
              <th>{{ jogador.name }}</th>
              <th>{{ jogador.n_camisa }}</th>
              <th>{{ jogador.time }}</th>
              <th>Bah</th>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
</template>
<style scoped></style>

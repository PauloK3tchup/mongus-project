<script>
import { v4 as uuid } from "uuid";
export default {
  novo_jogador: "",
  n_camisa: "",
  data() {
    return {
      jogadores: [
        {
          id: "0cbc9fa1-914b-4c30-ac39-3678396c79da",
          name: "Jogador 1",
          n_camisa: 1,
          time: 1,
        },
        {
          id: "f8b6464f-4d13-457d-bf4f-7fad84cd61e4",
          name: "Jogador 2",
          n_camisa: 2,
          time: 2,
        },
        {
          id: "da71a59c-0432-40d1-9d6a-3f9416f3cc61",
          name: "Jogador 3",
          n_camisa: 3,
          time: 3,
        },
        {
          id: "c5a9c485-1704-47a0-9183-f3fef961947c",
          name: "Jogador 4",
          n_camisa: 4,
          time: 4,
        },
      ],
    };
  },
  methods: {
    salvar() {
      const novo_id = uuid();
      this.jogadores.push({
        id: novo_id,
        name: this.novo_jogador,
        n_camisa: this.n_camisa,
        time: "WIP",
      });
    },
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
        <input
          type="text"
          name=""
          id=""
          placeholder="Nome do Jogador"
          v-model="novo_jogador"
        />
        <input type="text" name="" id="" placeholder="Time" />
        <input
          type="text"
          name=""
          id=""
          placeholder="Número da camisa"
          v-model="n_camisa"
        />
        <button @click="salvar">Salvar</button>
      </div>
      <div class="list-items">
        <table>
          <thead>
            <tr>
              <th>ID</th>
              <th>Nome</th>
              <th>N° Camisa</th>
              <th>Time ID</th>
              <th>Função</th>
              <th>Ações</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="jogador in jogadores" :key="jogador.id">
              <th>{{ jogador.id }}</th>
              <th>{{ jogador.name }}</th>
              <th>{{ jogador.n_camisa }}</th>
              <th>{{ jogador.time }}</th>
              <th>
                <select name="Posição" id="">
                  <option value="">Indefinido</option>
                  <option value="">Zagueiro</option>
                  <option value="">Goleiro</option>
                  <option value="">Atacante</option>
                  <option value="">Teu Pai</option>
                </select>
              </th>
              <th><button>☠</button></th>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
</template>
<style scoped></style>

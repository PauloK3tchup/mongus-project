<script>
import { v4 as uuid } from "uuid";
export default {
  data() {
    return {
      novo_time: "",
      times: [
        { id: "313526bc-ffc9-444a-b77a-334bc7e5b7de", name: "Time 1" },
        { id: "45f3d289-e236-487b-b1ed-a807855492a0", name: "Time 2" },
        { id: "6c2f765d-f8ff-4100-8a6c-5abf2f71c455", name: "Time 3" },
        { id: "ef7f22d8-3333-41c5-b854-fa32787ab0b8", name: "Time 4" },
      ],
    };
  },
  methods: {
    salvar() {
      if (this.novo_time !== "") {
        const novo_id = uuid();
        this.times.push({
          id: novo_id,
          name: this.novo_time,
        });
        this.novo_time = "";
      } else {
        alert("cu");
      }
    },
    excluir(time) {
      const indice = this.times.indexOf(time);
      this.times.splice(indice, 1);
    },
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
    <div class="form-input">
      <input
        type="text"
        placeholder="Nome do time"
        id="nome_time"
        v-model="novo_time"
        @keypress.enter="salvar"
      />
      <button @click="salvar">Salvar</button>
    </div>
    <div class="list-items">
      <table>
        <thead>
          <tr>
            <th>ID</th>
            <th>Nome</th>
            <th>Ações</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="time in times" :key="time.id">
            <th>{{ time.id }}</th>
            <th>{{ time.name }}</th>
            <th>
              <button>✎</button>
              <button @click="excluir(time)">☠</button>
            </th>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  <div class="mrwhite">
    <img
      class="bobux"
      src="https://www.einerd.com.br/wp-content/uploads/2019/06/Walter-White-morreu-Breaking-Bad-capa.jpg"
      alt="er white"
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

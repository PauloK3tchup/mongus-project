<template>
  <div class="container">
    <!-- <img
      class="bobux"
      src="https://www.einerd.com.br/wp-content/uploads/2019/06/Walter-White-morreu-Breaking-Bad-capa.jpg"
      alt=""
    /> -->
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
    <div class="form-input">
      <input type="text" name="" id="" />
      <button>Salvar</button>
    </div>
    <div class="list-times">
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
            <th>Time 1</th>
            <th>Balls</th>
          </tr>
          <tr>
            <th>2</th>
            <th>Time 2</th>
            <th>Nuts</th>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<style>
/* img.bobux {
  width: 1%;
  height: auto;
  transition: 0.1s;
  opacity: 0;
}

img.bobux:hover {
  transform: scale(100);
  opacity: 100%;
} */

.title {
  text-align: center;
  margin: 2rem 0;
}

.form-input {
  display: flex;
  justify-content: center;
}

.form-input input {
  width: 50%;
  border: 1px solid black;
  border-radius: 10px;
  padding: 0 0.5rem;
  height: 40px;
}

.form-input button {
  height: 40px;
  margin-left: 1%;
  background-color: crimson;
  font-weight: bold;
  color: white;
  border-radius: 10px;
  width: 10%;
  transition: 0.25s;
  border: 0px;
}

.form-input button:hover {
  background-color: rgb(85, 91, 255);
  box-shadow: rgb(85, 91, 255) 0px 0px 0px 1px, rgb(31, 193, 27) 0px 0px 0px 3px,
    rgb(255, 217, 19) 0px 0px 0px 5px, rgb(255, 156, 85) 0px 0px 0px 7px,
    rgb(255, 85, 85) 0px 0px 0px 9px;
}
</style>

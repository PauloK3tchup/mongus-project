<template>
  <main>
    <div class="container">
      <div class="title">
        <h2>Gerenciamento de Jogadores</h2>
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
              <th>N° Camisa</th>
              <th>Time</th>
              <th>Ações</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <th>1</th>
              <th>Neymar Sr.</th>
              <th>69</th>
              <th>Cockrinthians</th>
              <th>Bah</th>
            </tr>
            <tr>
              <th>2</th>
              <th>Rolandinho Carioca</th>
              <th>420</th>
              <th>Palmeiras</th>
              <th>Bah</th>
            </tr>
            <tr>
              <th>3</th>
              <th>Cristaldo Ronano</th>
              <th>2</th>
              <th>Farmengro</th>
              <th>Bah</th>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
</template>
<style>
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

.list-times {
  display: flex;
  justify-content: center;
  margin: 2rem 0;
}

table {
  width: 50%;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(0, 0, 0) 0px 0px 0px 3px;
  border-collapse: collapse;
  text-align: center;
}

table thead {
  background-color: rgb(0, 0, 0);
  color: white;
}

table thead th {
  font-weight: bolder;
}

table tbody tr:nth-child(odd) {
  background-color: crimson;
  color: white;
}
</style>

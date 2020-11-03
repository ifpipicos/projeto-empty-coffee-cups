<template>
  <card>
    <b-row align-v="center" slot="header">
      <b-col cols="8">
        <h3 class="mb-0">Lista de professores</h3>
      </b-col>
      <b-col cols="4" class="text-right"> 
      <a href="#!" class="btn btn-sm btn-primary">Cadastrar professores</a>
      <div class="text-right">
        <table class="table">
          <thead>
            <tr>
              <th scope="col">#</th>
              <th scope="col">Matrícula</th>
              <th scope="col">Nome</th>
              <th scope="col">Disciplina</th>
              </tr>
          </thead>
        </table>
      </div>
        <!--<div id="app">
          <div class="col-2">
            <label>Nome</label>
            <input v-model="contact.name" />
            <label>Telefone</label>
            <input type="number" v-model="contact.telephone" />

            <button class="mt-3 mb-3 btn btn-primary" @click="add()">
              Adicionar
            </button>
          </div>

          <table class="table">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">Nome</th>
                <th scope="col">Telefone</th>
                <th scope="col">Ação</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="item in list">
                <th scope="row">{{ item.id }}</th>
                <td>{{ item.name }}</td>
                <td>{{ item.telephone }}</td>
                <td>
                  <button @click="edit(item)" class="btn btn-info">
                    Editar
                  </button>
                  <button @click="remove(item)" class="btn btn-danger">
                    Excluir
                  </button>
                </td>
              </tr>
            </tbody>
          </table-->
        </div>
      </b-col>
    </b-row>
  </card>
</template>
<script>
export default {
  //Novo instância do Vue
  /*data() {
    return {
      const: (list = new Vue({
        el: "#app",
        contact: {
          id: 1,
          name: "fernando",
          telephone: "32423",
        },
        index: null,
        list: [],
      })),
    };
  },
  //Âncora do ciclo de vida do Vue
  mounted() {
    const contacts = JSON.parse(localStorage.getItem("contacts"));
    this.list = contacts ? contacts : [];
  },
  //Espaço para criação dos métodos
  methods: {
    add() {
      if (this.contact.id === 0) {
        this.contact.id = this.list.length + 1;
        this.list.push(this.contact);
      } else {
        this.list[this.index] = this.contact;
      }
      localStorage.setItem("contacts", JSON.stringify(this.list));
      this.contact = { id: 0, name: null, telephone: null };
    },

    remove(item) {
      const idx = this.list.indexOf(item);
      this.list.splice(idx, 1);
      localStorage.setItem("contacts", JSON.stringify(this.list));
    },

    edit(item) {
      this.index = this.list.indexOf(item);
      this.contact = Object.assign({}, item);
      localStorage.setItem("contacts", JSON.stringify(this.list));
    },
  },*/
};
</script>
<style></style>

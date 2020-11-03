<template>
  <card>
    <b-row align-v="center" slot="header">
      <b-col cols="8">
        <h3 class="mb-0">Cadastro</h3>
      </b-col>
      <b-col cols="4" class="text-right">
        <a href="#!" class="btn btn-sm btn-primary">Configurações</a>
      </b-col>
    </b-row>

    <b-form @submit.prevent="updateProfile">
      <h6 class="heading-small text-muted mb-4">Cadastro de professores</h6>

      <div class="pl-lg-4">
        <b-row>
          <b-col lg="6">
            <base-input
              type="text"
              label="Nome *"
              placeholder="Nome"
              v-model="user.username"
            >
            </base-input>
          </b-col>

          <b-col lg="6">
            <base-input
              type="text"
              label="Apelido"
              placeholder="Ex.: João"
              v-model="user.NickName"
            >
            </base-input>
          </b-col>

          <b-col lg="6">
            <base-input
              type="email"
              label="E-mail *"
              placeholder="professor@email.com"
              v-model="user.email"
            >
            </base-input>
          </b-col>
        </b-row>

        <hr class="my-4" />

        <h6 class="heading-small text-muted mb-4">
          Informações sobre o docente
        </h6>

        <b-row>
          <b-col lg="6">
            <base-input
              type="text"
              label="Área de atuação *"
              placeholder="Informática"
              v-model="user.discipline"
            >
            </base-input>
          </b-col>

          <b-col lg="6">
            <base-input
              type="time"
              label="Carga Horária"
              placeholder="12:00"
              v-model="user.workload"
            >
            </base-input>
          </b-col>
        </b-row>
      </div>

      <!--<hr class="my-4" />

       Address 
      <h6 class="heading-small text-muted mb-4">Informações de contato</h6>

      <div class="pl-lg-4">
        
        <b-row>
          <b-col lg="4">
            <base-input
              type="text"
              label="City"
              placeholder="City"
              v-model="user.city"
            >
            </base-input>
          </b-col>
          <b-col lg="4">
            <base-input
              type="text"
              label="Country"
              placeholder="Country"
              v-model="user.country"
            >
            </base-input>
          </b-col>
          <b-col lg="4">
            <base-input
              label="Postal Code"
              placeholder="ZIP Code"
              v-model="user.postalCode"
            >
            </base-input>
          </b-col>
        </b-row>
      </div>

      <hr class="my-4" />
      < Description 
      <h6 class="heading-small text-muted mb-4">About me</h6>
      <div class="pl-lg-4">
        <b-form-group
          label="About Me"
          label-class="form-control-label"
          class="mb-0"
          label-for="about-form-textaria"
        >
            <label class="form-control-label">About Me</label> 
          <b-form-textarea
            rows="4"
            value="A beautiful premium dashboard for BootstrapVue."
            id="about-form-textaria"
            placeholder="A few words about you ..."
          ></b-form-textarea>
        </b-form-group>
      </div>
      -->
    </b-form>
  </card>
</template>
<script>
export default {
  data() {
    return {
      user: {
        company: "Creative Code Inc.",
        username: "",
        email: "",
        NickName: "",
        discipline: "",
        workload: ""
      }
    };
  },
  methods: {
    updateProfile() {
      alert("Your data: " + JSON.stringify(this.user));
    }
  }
};
</script>
<style></style>

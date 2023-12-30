<template>
  <div class="home">
    <div class="row mx-0">
      <div class="col-lg-6">
        <div class="img-cont">
          <img alt="Logo" src="../assets/img/devbook.svg">
            <h3 class="text-center text-lg-center">Conéctate con el resto del mundo usando devbook</h3>
          </div>
        </div>
      <div class="col-lg-6">
        <card-comp :btns="btnArray" class="mx-auto card-comp">
          <template #default>
          <form>
            <div class="mb-3 mt-2">
                <input type="email" class="form-control" placeholder="name@example.com" />
            </div>
            <div class="mb-3 mt-2">
                <input type="password" class="form-control" placeholder="Contraseña" />
            </div>
          </form>
        </template>
        <template #footer>
          <hr/>
          <button class="btn btn-success">Crear cuenta</button>
        </template>
        </card-comp>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import CardComp from '../components/CardComp.vue'
    export default {
    name: 'HomeView',
    components: {
      CardComp
    },

    data() {
      return {
        btnArray: [
          {
            txt: 'Iniciar sesión',
            class: 'btn-primary',
          },
          {
            txt: 'Olvidaste tu contraseña?',
            class: '',
          },

      ],
      }
    },
}
</script>

<style scoped>
  .home {
    max-width: 895;
    margin: auto;
  }

  .img-cont {
    display: flex;
    flex-direction: column;
  }

  img {
    max-width: 800px;
  }

  .card-comp {
    max-width: 398px;
    margin-top: 2.6em;
  }

  .btn-success {
    margin: auto;
    min-width: 195px;
  }


  @media (min-width: 992px) {
    .home {
      margin: 2em auto;
    }
    img {
      margin: 0;
      margin-top: 1em;
      margin-left: 4rem;
    }
    h3 {
      margin: 1rem;
      margin-top: -2.3em;
      margin-left: 2em;
    }
  }
</style>

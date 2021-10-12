<template>
  <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades!</p>
  <p>Utilizo as seguintes tecnologias para Backend :</p>
  <ul v-for="technology in backend_technologies">
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>
  <div>
    <button @click="showEmail">Mostrar e-mail</button>
  </div>
  <p v-show="mostrar_email">Mande uma mensagem para: matheus@email.com</p>
  <p class="teste">Para acessar meu portfólio <a v-bind:href="url_portfolio">basta clicar aqui</a></p>
  <Picture />
</template>
<script>
import Picture from './Picture'
export default {
  name: 'Info',
  components: {
    Picture
  },
  data() {
    return { 
      esta_trabalhando: false,
      mostrar_email: false,
      email: 'joicevbarbosa@gmail.com',
      meu_link: 'https://www.google.com',
      textoBotao: 'Mostrar e-mail',
      backend_technologies: ['JavaScript','PHP', 'Python']
    }
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email
      if(this.mostrar_email) {
        this.textoBotao = 'Mostrar e-mail'
      }else {
        this.textoBotao = 'Esconder e-mail'
      }
    }
  }
}
</script>



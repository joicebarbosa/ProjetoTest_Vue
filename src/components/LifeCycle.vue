<template>
  <h1>Meu nome é {{ nome }}</h1>
  <Info />
</template>

<script>
import Info from './Info.vue'
export default {
  name: 'LifeCycle',
  components: {
    Info
  },
  data() {
    return { 
      nome: "Joice"
    }
  },
  created() {
    this.nome = "Matheus"
  }
}
</script>
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
    this.nome = 'Joice';
  }, 1000:
  this. lifeCycle()  
};

  mounted() {
   setTimeout(() => {
    this.nome = 'Pedro'
    }, 2000;)
    methods: {
    lifeCycle() {
      cosole.log("Executou");

    }
  }
}
</script>
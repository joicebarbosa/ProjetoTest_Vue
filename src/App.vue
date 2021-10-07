<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
  </div>
</template>

<script>
import PrimeiroComponente from '../../src/components/PrimeiroComponente.vue'
import LifeCycle from '../../src/components/LifeCycle.vue'
export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle
  }
}
</script>

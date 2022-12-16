

<script>
import TestComponent from './components/TestComponent.vue'
import CounterComponent from './components/CounterComponent.vue'
import ComputedComponent from './components/ComputedComponent.vue'
import SeacrhList from './components/SeacrhListComponent.vue'



export default {
  name: 'App',
  components: {
    TestComponent, 
    CounterComponent,
    ComputedComponent,
    SeacrhList
  }
}
</script>


<template>
  <div class="container">
    <test-component/>
    <CounterComponent/>
    <ComputedComponent/>
    <seacrh-list/>
  </div>
</template>

<style scoped>
  .container {
    margin: 0 auto;
    width: 700px;
    height: 100vh;
    display: flex;
    justify-content: center;
    flex-direction: column;
    
  }

  span {
    color: black;
  }
</style>


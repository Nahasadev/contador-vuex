<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>Hola</h1>
    <p> {{message}} {{$store.state.counter}} </p>
    <counter></counter>
  </div>
</template>

<script>
import Counter from '@/components/counter'
export default {
  name: 'app',
  components: {
    Counter
  },
  data () {
    return {
      message: 'HOLA COMPONENTE'
    }
  }
}

</script>

<style scoped lang="stylus">
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px
</style>

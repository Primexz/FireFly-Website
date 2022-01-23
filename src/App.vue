<template>
  <Header/>

  <Main />

  <Commands />
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Mainpage.vue'
import Commands from './components/Commands.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Commands
  }
}
</script>

<style>

</style>

<template>
  <div id="app">
    <Header/>
    <Profiles v-bind:dinosArray="dinos"/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header'
import Profiles from './components/Profiles'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Profiles,
    Footer
  },
  
}
</script>

<style>

</style>

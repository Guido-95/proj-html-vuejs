<template>
  <div id="app">
    <Header :listaHeader = 'listaHeader' :icone = "iconeHeader"/>
    <Main/>
    
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data(){
    return{
      listaHeader:['Home','Landing','Pages','Docs'],
     
    }
  }
}
</script>

<style lang="scss">

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {

  font-family: 'Nunito', sans-serif;;
  }

.wrapper{
  max-width: 1170px;
  
  margin: auto;
  
}

</style>

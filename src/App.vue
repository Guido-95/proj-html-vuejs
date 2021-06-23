<template>
  <div id="app">

    <Header :listaHeader = 'listaHeader' :logo='logo' />
    <Main/>
    
    <Footer :listaFooterSinistra='listaFooterSinistra' :listaFooterDestra='listaFooterDestra' :logoFooter ="logoFooter" />
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
      logo: 'logo-dark.png' ,
      listaHeader:['Home','Landing','Pages','Docs'],
      logoFooter: 'logo-light.png',
      listaFooterSinistra:['About us','Services','Team','Pricing','Project', 'Careers','Blog','Login'],
      listaFooterDestra:['Terms of Services','Privacy Policy','Documentation','Changelog','Components']
     
    }
  }
}
</script>

<style lang="scss">
html{
  scroll-behavior: smooth;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {

  font-family: 'Nunito', sans-serif;
}

h1,h2,h3{
  color: #161c2d;
}

.wrapper {
  max-width: 1170px;
  margin: auto;
  
}

.colore-paragrafo{
  font-weight: 600;
  color: #8492a6;
}

.testo-importante{
  font-weight: bold;
  color: #3157d4;
}

*:hover{
  transition: 0.2s;
}
</style>

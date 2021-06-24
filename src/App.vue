<template>
  <div id="app">
    <!-- header -->
    <Header :listaHeader = 'listaHeader' :logo='logo' />
    <!-- /header -->

    <!-- Main -->
    <Main/>
    <!-- /Main -->

    <!-- Footer -->
    <Footer :listaFooterSinistra='listaFooterSinistra' :listaFooterDestra='listaFooterDestra' :logoFooter ="logoFooter" />
    <!-- Footer -->
  </div>
</template>

<script>
// import componenti
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
      // logo header
      logo: 'logo-dark.png' ,
      // lista link header
      listaHeader:[
        {
          testo:"Home",
          link:'#',
          attivo: false
        },
        {
          testo:"Landing",
          link:'#',
          attivo: true
        },
        {
          testo:"Page",
          link:'#',
          attivo: false
        },
        {
          testo:"Docs",
          link:'#',
          attivo: false
        }
      ],

      // logo footer
      logoFooter: 'logo-light.png',
      // lista link sinistra footer
      listaFooterSinistra:['About us','Services','Team','Pricing','Project', 'Careers','Blog','Login'],
      // lista link destra footer
      listaFooterDestra:['Terms of Services','Privacy Policy','Documentation','Changelog','Components']
     
    }
  }
}
</script>

<style lang="scss">
html {
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

h1,h2,h3 {
  color: #161c2d;
}

.wrapper {
  max-width: 1170px;
  margin: auto; 
}

.colore-paragrafo {
  font-weight: 600;
  color: #8492a6;
}

.testo-importante {
  font-weight: bold;
  color: #3157d4;
}

*:hover {
  transition: 0.2s;
}
</style>

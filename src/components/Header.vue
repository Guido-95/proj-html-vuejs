<template>
    <header>
        <div class="wrapper">
            <div class="header-top">

                <!-- logo header -->
                <div class="logo">
                  <a href="index.html"> <img id="inizio-pagina" :src="require('../assets/img/' + logo)" alt=""> </a>  
                </div>
                <!-- /logo header -->

                <!-- link al centro -->
                <div class="menu-header">
                    <ul>
                        <li v-for="elemento,indicatore in listaHeader" :key="indicatore">
                                <!-- se è il secondo link della lista dagli la classe attivo -->
                            <a @click = "impostaAttivo(indicatore)" :class="elemento.attivo ? 'attivo' : 'non-attivo'" :href="elemento.link">

                                {{ elemento.testo }}

                                                                <!-- se è il primo elemento della lista togli la freccia -->
                                <i class="fas fa-chevron-down" :class="elemento == listaHeader[0] ? 'display-none' : ''"></i>
                            </a>
                        </li>
                    </ul>
                </div>
                <!-- /link al centro -->
                <!-- icone a destra -->
                <div class="icone-header">
                    <ul>
                        <li class="cerca">
                            <i class="fas fa-search"></i>
                        </li>
                        <li class="background-icona">
                            <i class="fab fa-github"></i>
                        </li>
                        <li class="background-icona">
                            <i class="fab fa-stack-overflow"></i>
                        </li>
                        <li class="background-icona">
                            <i class="far fa-user"></i>
                        </li>
                    </ul>
                </div>
                <!-- /icone a destra -->

            </div>
        </div>
        <!-- componente Jumbotron -->
        <Jumbotron/>
        <!-- /componente Jumbotron -->
    </header>
   
</template>

<script>
// import componenti
import Jumbotron from './Jumbotron.vue'

export default {
    name:'Header',
    components:{
        Jumbotron,
    },
    props:{
        // lista link header e logo
        listaHeader : Array,
        logo:String   
    },
    methods:{
        impostaAttivo(indicatore){
            this.listaHeader.forEach(
                element => {
                element.attivo = false;
                this.listaHeader[indicatore].attivo = true
            });
        }
    }
}
</script>

<style lang='scss' scoped>
.attivo {
    color: #3157d4;
}

.non-attivo{
    color: #3c4858;
}

.display-none{
    display: none;
}
header {
    background-color: #f8f9fc;
    
    .wrapper{
        .header-top{
            height: 70px;
            justify-content: space-between;
            display: flex;
            align-items: center;

            .logo {

                img {
                    width: 130px;
                }
            }
            .menu-header {
                ul {
                    display: flex;
                    justify-content: space-between;
                
                    li {
                        margin-right: 50px;

                        a {
                            text-decoration: none;

                            &:hover{
                                color: #3157d4;

                            }
                        }
                    }
                }
            }
            .icone-header {
                
                .cerca {
                    font-size: 17px;
                    margin-right: 15px;
                    cursor: pointer;
                    color: #8492a6;
                }

                ul  {

                    li {
                        margin: 4px;
                    }
                }

                .background-icona {
                    font-size: 18px;
            
                    i {  
                        box-shadow: 0px 0px 1px rgb(161, 161, 161), 0px 5px 4px #d2daf6;
                        border-radius: 5px;
                        color: #2f55d4;
                        background-color: #e4e9f8;
                        padding: 9px 10px;
                        cursor: pointer;

                        &:hover {
                            color:#e4e9f8 ;
                            background-color: #2f55d4;
                        }
                    }
                }
                
            }
            .menu-header,
            .icone-header {
                
                ul {
                    list-style: none;
                    display: flex;
                    align-items: center;

                    li {
                        font-size: 13px;
                        font-weight: 800;
                        text-transform: uppercase ;
                        
                    }
                }
            }
        }
        
    }
}
   
   
</style>
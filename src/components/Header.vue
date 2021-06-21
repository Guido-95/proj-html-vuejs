<template>
    <header>
        <div class="wrapper">
            <div class="header-top">

                <!-- logo header -->
                <div class="logo">
                    <img src="../assets/img/logo-dark.png" alt="">
                </div>
                <!-- menu centrale -->
                <div class="menu-header">
                    <ul>
                        <li v-for="elemento,indicatore in listaHeader" :class="elemento == listaHeader[1] ? 'attivo' : 'non-attivo'" :key="indicatore">
                            {{ elemento }} <i class="fas fa-chevron-down" :class="elemento == listaHeader[0] ? 'display-none' : ''"></i>
                        </li>
                     
                    </ul>
                </div>
                <!-- icone a destra -->
                <div class="icone-header">
                    <ul>
                        <li class="cerca">
                            <i class="uil uil-search"></i>
                        </li>
                        <li class="background-icona">
                            <i class="uil uil-github"></i>
                        </li>
                        <li class="background-icona">
                            <i class="uil uil-github"></i>
                        </li>
                        <li class="background-icona">
                            <i class="uil uil-github"></i>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
        <Jumbotron/>
    </header>
   
</template>

<script>
import Jumbotron from './Jumbotron.vue'


export default {
    name:'Header',
    components:{
        Jumbotron,
        
    },
    props:{
        listaHeader : Array,      
    }
}
</script>

<style lang='scss'>
.attivo{
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
                .logo{

                    img{
                        width: 130px;
                    }
                }
                .menu-header{
                    ul{
                        li{
                            margin: 10px;
                          
                        }
                    }
                }
                .icone-header{
                    ul{
                        li{
                            margin: 4px;
                        }
                    }
                    .background-icona{
                        font-size: 25px;
                        
                        
                        i{  
                            border-radius: 5px;
                            background-color: lightgray;
                            padding: 5px 8px;
                        }
                    }
                    
                }
                .menu-header,
                .icone-header{
                    ul{
                        .cerca{
                            font-size: 25px;
                            margin-right: 15px;
                        }
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
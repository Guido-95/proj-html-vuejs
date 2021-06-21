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
                        <li v-for="elemento,indicatore in listaHeader" :class="elemento == listaHeader[1] ? 'attivo' : '' " :key="indicatore">
                            {{ elemento }} <i class="fas fa-chevron-down"></i>
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
    </header>
   
</template>

<script>

export default {
    name:'Header',
   
    props:{
        listaHeader : Array,
        iconeHeader: Array,        
    }
}
</script>

<style lang='scss'>
.attivo{
    color: blue;
}
    header {
        height: 500px;
        background-color: lightgrey;
        
        .wrapper{

            .header-top{
                height: 70px;
                background-color: lightseagreen;
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
                            font-weight: 700;
                            text-transform: uppercase ;
                            
                        }
                    }
                }
            }
            
        }
    }
   
   
</style>
<template>
<!-- div contenitore col bordo -->
<div class="border-bottom">
    <!-- div in position absolute con l'ingranaggio -->
    <div class="impostazioni">
        <i class="fas fa-cog"></i>
    </div>
    <!-- div in position absolute con l'ingranaggio -->

    <!-- div contenitore rientrato -->
    <div class="wrapper">
        <!-- jumbotron -->
        <div class="jumbotron">
            <div class="testo-jumbotron">
                <span class="bottone-arrotondato"> 
                    Development 
                </span>
                <!-- h1 jumbotron -->
                <h1>
                    A Complete Developer Toolset 
                </h1>
                <!-- -h1 jumbotron -->
                <p class = "parargrafo-jumbotron colore-paragrafo">
                    Launch your campaign and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.
                </p>
                <button class="bottone bottone-background"> Get started </button> 
                <button class="bottone bottone-no-background"> Documentation </button>
                <div class="versione"> Current Version: v2.6.0 </div>
            </div>
        </div>
        <!-- -jumbotron -->
    </div>
    <!-- div contenitore rientrato -->
</div>
<!-- div contenitore col bordo -->

   
</template>

<script>
export default {
    name:'Jumbotron'
}
</script>

<style lang='scss' scoped>

.border-bottom {
    padding-top: 80px;
    padding-bottom: 80px;
    position: relative;
    border-bottom: 1px solid #e9ecef;

    .impostazioni {
        position: absolute;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        top: 50px;
        left: -60px;
        width: 100px;
        border-radius: 20px;
        padding: 10px;
        cursor: pointer;
        background-color: white;
        box-shadow: 0px 0px 2px lightgray;

        i {  
            font-size: 20px;
            color: #3157d4;
        }
    }

    .jumbotron {
        display: flex;
        align-items: center;
        height: 500px;
        background-repeat: no-repeat;
        background-position: 96% 70%;
        background-size: 42% 95%;
        background-image: url('../assets/img/about.png');

        .bottone-arrotondato {
            display: inline-block;
            border-radius: 20px;
            margin-bottom: 10px;
            border: 1px solid lightgray;
            padding: 2px 10px;
            font-size: 12px;
            font-weight: 800;
            background: #e4e9f8;
            color: #3157d4;
        }
        .testo-jumbotron {
            width: 48%;

                h1 {
                font-weight: 800;
                width: 70%;
                font-size: 40px;
                padding-right: 5px;
            }
            .parargrafo-jumbotron {
                margin: 25px 0px;
                font-weight: 600;
                font-size: 18px;
            }
            .versione {
                margin-top: 5px;
                font-weight: 600;
                font-size: 15px;
                color: #8b98ab;
            }
            .bottone {
                margin: 0px 10px 10px 0px;
                font-family: 'Nunito', sans-serif;
                border: none;
                border-radius: 5px;
                padding: 10px 20px;
                font-weight: 700;
                font-size: 16px;
                cursor: pointer;
            }
            .bottone.bottone-background {
                box-shadow:0px 1px 3px #2443ac;
            }
            .bottone.bottone-background:hover {
                background-color: #2443ac;
            }
            .bottone-background {
                background-color: #2f55d4;
                color: white;
            }
            .bottone-no-background {
                border: 1px solid #2f55d4;
                color: #2f55d4;
                
                &:hover {
                    color:white;
                    background-color:#2f55d4;
                }
            }
            
            
        } 
    }
}
</style>
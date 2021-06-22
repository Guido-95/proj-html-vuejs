<template>
<div class="border-bottom">
    <div class="impostazioni">
        <i class="fas fa-cog"></i>
    </div>
    <div class="wrapper">
        
        <div class="jumbotron">
            <div class="testo-jumbotron">
                <span class="bottone-arrotondato"> Development </span>
                <h1>A Complete Developer Toolset </h1>
                <p class="parargrafo-jumbotron colore-paragrafo">Launch your campaign and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.</p>
                <button class="bottone bottone-background">Get started</button> 
                <button class="bottone bottone-no-background">Documentation</button>
                <div class="versione">Current Version: v2.6.0</div>
            </div>
        </div>
    </div>
</div>

   
</template>

<script>
export default {
    name:'Jumbotron'

}
</script>

<style lang='scss' scoped>
.border-bottom {
    position: relative;
    border-bottom: 1px solid lightgrey;
    .impostazioni{
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
        i{  
            font-size: 20px;
            color: #3157d4;
        }
    }
}
    .jumbotron {
        display: flex;
        align-items: center;
        height: 500px;
        background-repeat: no-repeat;
        background-position: 96% 70%;
        background-size: 30% 70%;
        background-image: url('../assets/img/about.png');
        .bottone-arrotondato{
            border-radius: 20px;
            background: #e4e9f8;
            border: 1px solid lightgray;
            padding: 2px 10px;
            font-size: 12px;
            font-weight: 800;
            color: #3157d4;
        }
        .testo-jumbotron {
            width: 41%;
            .parargrafo-jumbotron {
                margin: 25px 0px;
                font-weight: 600;
                font-size: 15px;
            }
            .versione{
                font-weight: 600;
                font-size: 14px;
                color: #8b98ab;
            }
            .bottone{
                margin: 0px 10px 10px 0px;
                font-family: 'Nunito', sans-serif;
                border: none;
                border-radius: 5px;
                padding: 10px 20px;
                font-weight: 700;
                font-size: 16px;
                cursor: pointer;
                
            }
            .bottone.bottone-background:hover{
                background-color: #2443ac;
            }
            .bottone-background{
                background-color: #2f55d4;
                color: white;
            }
            .bottone-no-background{
                border: 1px solid #2f55d4;
                color: #2f55d4;
                
                &:hover{
                    color:white;
                    background-color:#2f55d4;
                }
            }
            h1 {
                font-size: 46px;
                padding-right: 5px;
            }
            
        } 
    }
</style>
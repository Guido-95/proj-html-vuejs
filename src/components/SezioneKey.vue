<template>
    <div class="wrapper">
        <div class="intestazione">
            <h2>Key Features</h2>
            <p class="colore-paragrafo">Start working with <span class="testo-importante"> Landrick  </span>that can provide everything need to generate awareness, drive traffic, connect.</p>
        </div>
        <div class="colonne">
            <div class="colonna">
                <div class="icona">
                    <i class="uil uil-layer-group"></i>
                </div>
                <h4 >Modular</h4>
                <p class="colore-paragrafo">Composed in a pseudo-Latin language which more or less corresponds.

                </p>
                <span>Read more <i class="fas fa-chevron-right"></i> </span>
            </div>
            <div class="colonna">
                <div class="icona">
                    <i class="uil uil-airplay"></i>
                </div>
                <h4>Responsive</h4>
                <p class="colore-paragrafo">Composed in a pseudo-Latin language which more or less corresponds.</p>
                <span>Read more <i class="fas fa-chevron-right"></i> </span>
            </div>
            <div class="colonna">
                <div class="icona">
                    <i class="uil uil-focus-target"></i>
                </div>
                <h4>Customizable</h4>
                <p class="colore-paragrafo">Composed in a pseudo-Latin language which more or less corresponds.</p>
                <span>Read more <i class="fas fa-chevron-right"></i> </span>
            </div>
            <div class="colonna">
                <div class="icona">
                    <i class="uil uil-expand-arrows"></i>
                </div>
                <h4>Scalable</h4>
                <p class="colore-paragrafo">Composed in a pseudo-Latin language which more or less corresponds.</p>
                <span> Read more <i class="fas fa-chevron-right"></i> </span>
            </div>
        </div>
        <div class="parte-bassa">
            <h4>Quickstart</h4>
            <h2>
                Awesome isn't it? let's dive in!
            </h2>
            <p class="colore-paragrafo">Start working with <span class="testo-importante"> Landrick  </span> that can provide everything need to generate awareness, drive traffic, connect.</p>

            <div class="npm">
                <div class="contenitore-npm">
                    <div class="attivo">npm</div>
                    <div>nuget</div>
                    <div>spm</div>
                    <div>github</div>
                </div>
                <div class="parte-bassa-npm colore-paragrafo">
                   <span class="verde"> &dollar; </span>  npm install <span class="verde"> -g </span> claps.js
                </div>
                
              
            </div>
            <div class="check colore-paragrafo">
                <div> 
                    <i class="far fa-check-circle"></i> 
                    Organize your data
        
                </div>
                <div> 
                    <i class="far fa-check-circle"></i> 
                    Work with any team
        
                </div>
                </div>
            </div>
        
        

    </div>
</template>

<script>
export default {
name:'SezioneKey'
}
</script>

<style lang='scss' scoped>
.wrapper{

    .intestazione{
        width: 50%;

        h2{
            margin: 80px 0px 40px 0px;
            font-size: 30px;
        }
        p{
            margin-bottom: 50px;
            
        }
    }
    .colonne{
        display: flex;
        justify-content: space-between;
        h4{
            margin: 20px 0px 15px 0px;
        }
       
        .colonna{
            width: calc(100% / 4 - 20px);
          
            border-radius: 4px;
            padding: 32px 24px;
            margin-bottom: 50px;
            box-shadow: 0 0 5px #eaf0f6;
            


            p {  
                font-weight: 600;
            }
            span{
                display: block;
                margin: 20px 0px 0px 0px;
                color: #3157d4;

                i {
                    font-size: 10px;
                }
            }
            .icona i{
                
                border-radius: 5px;
                padding: 10px 20px;
                background-color: #eaeefb;
                font-size: 30px;
                color: #3157d4;
            }
        }
    }

     .parte-bassa{
        margin: auto;
        text-align: center;
        margin-bottom: 80px;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 60%;

        h2{
            font-size: 30px;
            
        }
        h4 {
            text-align: center;
            color: #3157d4;
        }
        p{
            width: 80%;
            margin-bottom: 70px;
        }
        .npm{
            padding: 25px 15px;
            width: 100%;
            border-radius: 5px;
            background-color: #3c4858;
            .contenitore-npm{
                margin: auto;
                width: 100%;
                display: flex;
                border: 1px solid #5a6474;
                background-color: #4f5a69;
                border-radius: 5px;
                .attivo{
                    border-radius: 8px;
                    height: 100%;
                    background-color: #3c4858;     
                }
                div {
                    font-size: 18px;
                    width: calc(100% / 4);
                    padding: 10px 32px;
                    color: white;
                }
            }
        }
        .parte-bassa-npm{
            margin-top: 20px;
            font-weight: 700;
            width: 100%;
            text-align:left;
            .verde{
                color: #4cd19b;
            }
        }
        
    }
    .check{
       
        width: 100%;
        display: flex;
        div{
            margin: 25px 50px 15px 0px;
        }
        i{  
            font-size: 15px;
            color: #4cd19b;
        }
    }

}

</style>
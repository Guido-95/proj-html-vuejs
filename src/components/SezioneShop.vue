<template>
  <div class="wrapper">
        <h2> Our rates for developer from landrick team </h2>
        <p class="colore-paragrafo testo-shop">Start working with <span class="testo-importante"> Landrick  </span>that can provide everything need to generate awareness, drive traffic, connect.</p>
        <div class="contenitore-colonne">
            <div class="colonna">
                <span class="bottone-arrotondato"> Basic </span>
                <div class="prezzo"> &dollar; 9.00</div>
                <div class="colore-paragrafo"> Per month </div>
                <div class="colore-paragrafo paragrafo-colonna"> All the basics for business that are just getting started. </div>
                
                <div class="check">
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Full Acces
                    </div>
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Source Files
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        1 Domain Free
                    </div>
                   
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>

                    <button class="bottone bottone-background">Buy Now</button>
                    <div class="colore-paragrafo">*No credit card required</div> 
                </div>
                
            </div>
            <div class="colonna">
              <div class="cover-ribbon">
                  <div class="cover-ribbon-inside"> Best </div>
              </div>
                <span class="bottone-arrotondato"> Business </span>
                <div class="prezzo"> &dollar; 39.00</div>
                <div class="colore-paragrafo"> Per month </div>
                <div class="colore-paragrafo paragrafo-colonna"> Better for growind businesses that want more customers. </div>
                
                <div class="check">
                   <div class="check-singolo colore-paragrafo ">
                        <i class="far fa-check-circle"></i> 
                        Full Acces
                    </div>
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Source Files
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        1 Domain Free
                    </div>
                   
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>

                    <button class="bottone bottone-background">Buy Now</button>
                    <div class="colore-paragrafo">*No credit card required</div> 
                </div>
            </div>
            <div class="colonna">
                <span class="bottone-arrotondato"> Enterprise </span>
                <div class="prezzo"> &dollar; 79.00</div>
                <div class="colore-paragrafo"> Per month </div>
                <div class="colore-paragrafo paragrafo-colonna"> Advanced feature for pros who need more customization. </div>
                
                <div class="check">
                    <div class="check-singolo colore-paragrafo ">
                        <i class="far fa-check-circle"></i> 
                        Full Acces
                    </div>
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Source Files
                    </div>
                     <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        1 Domain Free
                    </div>
                   
                    <div class="check-singolo colore-paragrafo">
                        <i class="far fa-check-circle"></i> 
                        Enhanced Security
                    </div>


                    <button class="bottone bottone-background">Buy Now</button>
                    <div class="colore-paragrafo">*No credit card required</div> 
                </div>
            </div>
    </div>
    
  </div>
</template>

<script>
export default {

}
</script>

<style lang='scss' scoped>
hr{
    width: 100%;
}
.wrapper{
    padding: 80px 0px;
    text-align: center;
    h2{
        font-size: 30px;
    }
    .colore-paragrafo{
       
        font-weight: 600;
    }
    .testo-shop{
        margin: auto;
        width: 50%;
    }
    .contenitore-colonne{
        margin-top: 50px;
        display: flex;
        justify-content: space-between;
        
        .colonna{
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0px 4px  #eaf0f6,  0 0 5px #eaf0f6;
            width: calc(100% / 3 - 30px);
            cursor: pointer;

            &:hover{
                box-shadow: 0px 4px  #2f55d4,  0 0 5px #eaf0f6;
                transform: scale(1.1);
                // transition: 0.5s;
                
            }
            .cover-ribbon {
                height: 115px;
                width: 115px;
                position: absolute;
                right: -8px;
                top: -8px;
                overflow: hidden;
            }
            .cover-ribbon .cover-ribbon-inside {
                background: #f17425;
                color: #FFF;
                transform: rotate(46deg);
                position: absolute;
                right: -35px;
                top: 20px;
                padding: 2px;
                width: 127px;
                text-align: center;
            }
            .cover-ribbon .cover-ribbon-inside:before {
                width: 0;
                height: 0;
                border-left: 7px solid transparent;
                border-right: 7px solid transparent;
                border-bottom: 10px solid #992C23;
                position: absolute;
                left: -1px;
                right: 0;
                bottom: 0;
                content: "";
                top: 23px;
                transform: rotate(-45deg);
            }
            .cover-ribbon .cover-ribbon-inside:after {
            width: 0;
            height: 0;
            border-top: 7px solid transparent;
            border-left: 10px solid #992C23;
            border-bottom: 7px solid transparent;
            position: absolute;
            left: 88%;
            right: 0;
            top: 21px;
            bottom: 0;
            content: "";
            transform: rotate(-45deg);
            }
            .paragrafo-colonna{
                margin: 15px 0px 15px 0px;
                padding-bottom: 20px;
                border-bottom: 1px solid #cbd6e2;
            }
            .check{
                width: 100%;

                .bottone{
                    width: 100%;
                    margin: 20px 0px 20px 0px;
                    font-family: 'Nunito', sans-serif;
                    border: none;
                    border-radius: 5px;
                    padding: 10px 20px;
                    font-size: 15px;
                    font-weight: 700;
                    cursor: pointer;
                }
                .bottone.bottone-background:hover{
                    background-color: #2443ac;
                }
                .bottone-background{
                    background-color: #2f55d4;
                    color: white;
                }
                .check-singolo{
                    margin-top: 10px;
                    i{
                        color: #2f55d4;
                    }
                }
            }
            div{
                text-align: left;
            }
       
        .bottone-arrotondato{
            margin-bottom: 15px;
            border-radius: 18px;
            background: #eaeefb;
            padding: 8px 23px;
            box-shadow:  0 0 2px #eaf0f6;
            font-size: 15px;
            font-weight: 700;
            color: #3157d4;
        }
        .prezzo{
            margin-bottom: 5px;
            font-size: 30px;
            font-weight: 800;
        }
    }
    }
    
}
</style>
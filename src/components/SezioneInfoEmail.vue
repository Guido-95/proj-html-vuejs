<template>
  <div class="wrapper">
        <div class="email-info">
            <h3>
                Want to be among the first to find out?
            </h3>
            <p class="colore-paragrafo testo-shop">Start working with <span class="testo-importante"> Landrick  </span>that can provide everything need to generate awareness, drive traffic, connect.</p>
            <div class="email-bottone">
                <div class="email">
                    Email Address
                </div>
                <div class="bottone">
                   <button> Get Started </button> 
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
name:'SezioneInfoEmail'
}
</script>

<style lang='scss' scoped>
    .email-info {
        text-align: center;
        margin: auto;
        width: 50%;
        .colore-paragrafo{
            font-weight: 600;
        }
        h3{
            font-size: 29px;
            margin-bottom: 20px;
        }
        .email-bottone{
            box-shadow: 0px 0px 2px lightgray;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 4px 5px ;
            border-radius: 30px;
            margin-bottom: 90px;
            margin-top: 30px;
            width: 100%;
            font-weight: 600;
            .email{
                margin-left: 30px;
                color: #8896a9;
            }
            .bottone{
                button{
                    font-family: 'Nunito', sans-serif;
                    font-weight: 600;
                    font-size: 16px;
                    padding: 10px 20px;
                    border: none;
                    color: white;
                    border-radius: 30px;
                    background-color: #2f55d4;
                }
            }
        }
    }
</style>
<template>
    <!-- contenitore rientrato -->
    <div class="wrapper">
        <!-- div email col bottone -->
        <div class="email-info">
            <h2>
                Want to be among the first to find out?
            </h2>
            <p class="colore-paragrafo testo-shop">Start working with <span class="testo-importante"> Landrick  </span>that can provide everything need to generate awareness, drive traffic, connect.</p>
            <div class="email-bottone">
                <input type="text" class="email" placeholder="Email Address">
                <div >
                <button class="bottone"> Get Started </button> 
                </div>
            </div>
        </div>
        <!-- /div email col bottone -->
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

    .colore-paragrafo {
        font-weight: 600;
    }
    h2 {
        font-size: 29px;
        margin-bottom: 25px;
    }
    .email-bottone {
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

        .email {
            width: 50%;
            height: 30px;
            border: none;
            margin-left: 30px;
            font-size: 17px;
            color: #8896a9;

            &::placeholder {
                font-family: 'Nunito', sans-serif;
                font-size: 15px;
            }
            &:focus{
                outline: none;
            }
        }
        .bottone {
            cursor: pointer;
            font-family: 'Nunito', sans-serif;
            font-weight: 600;
            font-size: 16px;
            padding: 10px 20px;
            border: none;
            color: white;
            border-radius: 30px;
            background-color: #2f55d4;  
            box-shadow:0px 1px 2px #2443ac;
            
            &:hover {
            background-color: #2443ac;
            }
        }
        
    }
}
</style>
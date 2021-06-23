<template>
    <!-- contenitore rientrato -->
    <div class="wrapper">
        <!-- div sinistra tools con h2 - p -->
        <div class="div-sinistra">
            <h2>
                Build tools and extensive documentation
            </h2>
            <p class="colore-paragrafo">
                You can combine all the Landrick templates into a single one, you can take a component from the Application theme and use it in the Website.
            </p>
            <div class="colore-paragrafo">
                <i class="far fa-check-circle"></i> 
                Digital Marketing Solutions for Tomorrow 
            </div>
            <div class="colore-paragrafo">
                <i class="far fa-check-circle"></i> 
                Our Talented & Experienced Marketing Agency 
            </div>
            <div class="colore-paragrafo">
                <i class="far fa-check-circle"></i> 
                Create you own skin to match your brand 
            </div>
            <button class="bottone bottone-background">
                Read More <i class="fas fa-arrow-right"></i>
            </button> 
        </div>
        <!-- /div sinistra tools con h2 - p -->

        <!-- div destra tools con img -->
        <div class="div-destra">
            <img src="../assets/img/1.png" alt="grafico">
        </div>
        <!-- /div destra tools con img -->

    </div>
    <!-- /contenitore rientrato -->
</template>

<script>
export default {
name:'SezioneTools'
}
</script>

<style lang='scss' scoped>
.wrapper {
    display: flex;

    .div-sinistra {
        width: 60%;

        h2 {
            padding-top: 30px;
            width: 50%;
            font-size: 30px;
            margin-bottom: 25px;
        }
        p {
            font-weight: 600;
            width: 80%;
            margin-bottom: 20px;
        }
        div {
            font-weight: 600;
            margin-top: 10px;

            i {  
                margin-right: 10px;
                color: #2f55d4;
            }
        }
        .bottone {
            cursor: pointer;
            margin-top: 20px;
            font-family: 'Nunito', sans-serif;
            border: none;
            border-radius: 5px;
            padding: 10px 20px;
            font-size: 15px;
            font-weight: 700;
        }
        .bottone.bottone-background:hover {
            background-color: #2443ac;
        }
        .bottone-background {
            background-color: #2f55d4;
            color: white;
        }
        .fa-arrow-right {
            margin-left: 5px;
            font-size: 10px;
        }
        
    }
    .div-destra {
        width: 40%;

        img {
            width: 440px;
        }
    }

}
</style>